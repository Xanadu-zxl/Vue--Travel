<template>
	<div class="icons">
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>
		<div class="icon">
			<div class="icon-img">
				<img class="icon-img-content" src="https://pic.52112.com/icon_pack_thumb/201901/23131016_7af8bc94e1.png" alt="">
			</div>
			<p class="icon-desc">旅游景点</p>
		</div>

	</div>
</template>

<script>
	export default {
		name: 'HomeIcons'
		// 		props: {
		// 			list: Array
		// 		},
		// 		data() {
		// 			return {
		// 				swiperOption: {
		// 					autoplay: false
		// 				}
		// 			}
		// 		},
		// 		computed: {
		// 			pages() {
		// 				const pages = []
		// 				this.list.forEach((item, index) => {
		// 					const page = Math.floor(index / 8)
		// 					if (!pages[page]) {
		// 						pages[page] = []
		// 					}
		// 					pages[page].push(item)
		// 				})
		// 				return pages
		// 			}
		// 		}
	}
</script>

<style scoped>
	
	.icons {
		width: 100%;
		overflow: hidden;
		height: 0;
		padding-bottom: 50%;
	}

	.icon {
		position: relative;
		overflow: hidden;
		height: 0;
		float: left;
		width: 25%;
		padding-bottom: 25%;
	}

	.icon-img {
		position: absolute;
		top: 0;
		left: 0;
		right: 0;
		bottom: .44rem;
		box-sizing: border-box;
		padding: .1rem;
	}
	.icon-img-content {
		display: block;
		margin: 0 auto;
		height: 100%;
	}
	.icon-desc {
		position: absolute;
		left: 0;
		right: 0;
		bottom: 0;
		height: .44rem;
		line-height: .44rem;
		text-align: center;
		color: #333;
	}
</style>
