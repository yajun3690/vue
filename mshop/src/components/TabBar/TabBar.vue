<template>
	<div class="TabBar">
		<ul class="tab-bar-wrap">
			<li class="tab-bar-item">
				<router-link class='tab-bar-link' to='/home'
				>
					<i class="fa fa-home"></i>
					<span>首页</span>
				</router-link>
			</li>
			<li class="tab-bar-item">
				<router-link class='tab-bar-link' to='/cart'>
					<i class="fa fa-star"></i>
					<span>购物车</span>
				</router-link>
			</li>
			<li class="tab-bar-item">
				<router-link class='tab-bar-link' to='/me'>
					<i class="fa fa-user"></i>
					<span>个人中心</span>
				</router-link>
			</li>
		</ul>
	</div>
</template>
<script>
	export default {
		name:'TabBar',
		mounted(){

		}
	}	
</script>
<style  lang="less">
	.TabBar{
		position: fixed;
		left: 0;
		bottom: 0;
		width: 100%;
		.tab-bar-wrap{
			display: flex;
			flex-direction: row;
			justify-content: space-around;
			background-color: #ccc;
			.rem(padding,10,0);
			.tab-bar-link{
				.rem(font-size,18);
				display: flex;
				flex-direction: column;
				text-align: center;
				text-decoration: none;
				color: #333;
			}
			.tab-bar-link.active{
				color: #f21;
			}
		}
	}
</style>