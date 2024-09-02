<template>
	<view>
		<scroll-view class="scroll" scroll-x="true">
			<view class="item">1</view>
			<view class="item">2</view>
			<view class="item">3</view>
			<view class="item">4</view>
			<view class="item">5</view>
		</scroll-view>
		<swiper class="swiper" circular="true">
			<swiper-item class="item">滑块1</swiper-item>
			<swiper-item class="item">滑块2</swiper-item>
			<swiper-item class="item">滑块3</swiper-item>
		</swiper>
		<navigator url="/pages/index/index">点我跳转</navigator>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss">
	.scroll{
	
		border: 1px solid red;
		box-sizing: border-box;
		height: 200rpx;
		width: 750rpx;
		background-color: yellowgreen;
		white-space: nowrap;
		.item{
			width: 200rpx;
			height: 200rpx;
			background-color: blueviolet;
			display: inline-block;
			margin-right: 10rpx;
		}
	}
	.swiper{
		.item{
			background-color: pink;
		}
	}
</style>
