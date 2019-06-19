<template>
	<div class="wrapper">
		<swiper :options="swiperOption">
			<swiper-slide>
				<img class="swiper-img" src="https://f-flightfe-portalcp.qunarzz.com/f_flightfe_portal_f_flightfe_portal/2019/1547807426824_26157347.jpg"
				 alt="轮播图">
			</swiper-slide>
			<swiper-slide>
				<img class="swiper-img" src="https://f-flightfe-portalcp.qunarzz.com/f_flightfe_portal_f_flightfe_portal/2019/1547807426824_26157347.jpg"
				 alt="轮播图">
			</swiper-slide>
			<div class="swiper-pagination" slot="pagination"></div>
		</swiper>
	</div>
</template>

<script>
	export default {
		name: 'HomeSwiper',
		data() {
			return {
				swiperOption: {
					pagination: '.swiper-pagination',
					loop:true
				}
			}
		}
	}
</script>

<style scoped>
	.wrapper >>> .swiper-pagination-bullet-active{
		background:#FFFFFF;
	}
	.wrapper{
		width: 100%;
		height: 0;
		overflow: hidden;
		padding-bottom: 31.25%;
		background: #eee;
	}
	.swiper-img {
		width: 100%;
	}
</style>
