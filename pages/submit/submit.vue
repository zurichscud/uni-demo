<template>
	<view class="out">
		<view class="title">个人信息</view>
		<view class="row">
			<input type="text" placeholder="请输入姓名" v-model="message.name" />
		</view>
		<view class="row">
			<input type="text" placeholder="请输入联系电话" v-model="message.phone"/>
		</view>
		<view class="row">
			<textarea type="text" placeholder="请输入留言内容" v-model="message.content"/>
		</view>
		<view class="row">
			<button type="primary" @click="onSubmit">submit</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				message:{
					name:'',
					phone:'',
					content:''
				}
			};
		},
		methods:{
			onSubmit(){
				console.log(this.message)
			}
		}
	}
</script>

<style lang="scss">
	.out{
		padding: 30rpx;
		.title{
			margin-bottom: 20rpx;
		}
		.row{
			margin-bottom: 10rpx;
			border: 1px solid #eee;
			box-sizing: border-box;
			
		}
	}

</style>
