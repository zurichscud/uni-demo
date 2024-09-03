<template>
    <view>
		<text>导航高亮案例</text>
        <view class="nav">
			<view class="item" 
			:class="index==navIndex ? 'active':''" 
			v-for="(item,index) in navArr" 
			:key="item.id"
			@click="addActive(index)">{{item.title}}</view>
		</view>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                navArr:[
					{id:1,title:"Java"},
					{id:2,title:"Php"},
					{id:3,title:"Go"},
					{id:4,title:"C++"},
				],
				navIndex:0,
				
            }
        },
        methods: {
			addActive(index){
				this.navIndex=index
			}
            
        }
    }
</script>

<style lang="scss">
	.nav{
		display: flex;
		justify-content: space-around;
		background: #ccc;
		align-items: center;
		.item{
			flex: 1;
			line-height: 90rpx;
			text-align: center;
			&.active{
				background: red;
				color: #fff;
			}
		}
	}

</style>
