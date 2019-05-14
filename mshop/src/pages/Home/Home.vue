<template>
	<div class="Home">
		<div class="swiper-container">
			<div class="swiper-wrapper">
				<div class="swiper-slide">
					<img src="../../assets/images/1.jpg" alt="">
				</div>
				<div class="swiper-slide">
					<img src="../../assets/images/2.jpg" alt="">
				</div>
				<div class="swiper-slide">
					<img src="../../assets/images/3.jpg" alt="">
				</div>
			</div>
			<!-- 如果需要分页器 -->
			<div class="swiper-pagination"></div>
		</div>
	</div>
</template>
<script>
	import Swiper from 'swiper';
	import 'swiper/dist/css/swiper.min.css';
	export default {
		name:'Home',
		mounted(){
			new Swiper ('.swiper-container', {
				// 循环模式选项
				loop: true,
				autoplay:true,
				//分页器
				pagination: {
				  el: '.swiper-pagination',
				  clickable:true
				},
			})
		}
	}	
</script>
<style scoped lang="less">
	.Home .swiper-slide img{
		width: 100%;
		box-sizing: border-box;
		.rem(height,240)
	}
</style>