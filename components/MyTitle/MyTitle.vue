<template>
	<view>
		<view class="title">{{title}}</view>
		<view class="sub">{{subTitle}}</view>
		
	</view>
</template>

<script>
	export default {
		name:"MyTitle",
		props:["title","subTitle"],
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
	.title{
		font-size: 100rpx;
		text-align: center;
	}
	.sub{
		font-size: 50rpx;
		color: red;
		text-align: center;
	}

</style>