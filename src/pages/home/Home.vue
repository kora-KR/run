<template>
	<div>	
		<index-header/>
		<index-swiper/>
		<index-iconSwiper/>
		<index-activity />
 		<index-hotsale />
 		<index-weekend />
 	</div>
</template>

<script>
import Header from "./components/Header";
import Swiper from "./components/Swiper";
import IconSwiper from "./components/IconSwiper";
import Activity from "./components/Activity";
import Recommend from "./components/RecommendList";
import WeekendList from "./components/WeekendList";

export default {
	components: {
				"index-header": Header,
				"index-swiper":Swiper ,
				"index-iconSwiper": IconSwiper,
				"index-activity":Activity ,
				"index-hotsale":Recommend,
				"index-weekend":WeekendList

	},
	
	mounted(){
		// if( !this.$store.state.iconSwiper.length && 
		// 	!this.$store.state.iconSwiper1.length &&
		// 	!this.$store.state.swiperInfo.length){
		// 	 this.$store.dispatch("getSwiper");
		// }
			// if(this.$store.getters.shouldGetData){
			 	this.$store.dispatch("getSwiper");
			// }
		
	}
}

</script>

<style>
</style>



