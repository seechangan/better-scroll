<template>
	<div>
	     <views ref="scroll"  :scrollX="ThisX" :scrollY="ThisY" :data="ThisData">
		<div  class="scroll-content"></div>
	     </views>
	</div>
</template>

（import views from "./base/view-scroll" ） *注意,根据自己实际项目结构更改导入地址

export default {
  components: {views},
  data() {
    return {
       ThisX:false,//控制横向是否可滚动 
       ThisY:true,//控制竖向是否可滚动 
       ThisData:[],//根据solt中接收时所规定的类型来传递，默认是数组
    };
  }
};

