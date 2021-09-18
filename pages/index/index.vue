<template>
	<view class="cu-bar bg-grey bottom-wrapper margin-top">
			<view class="box">
				<view class="cu-bar tabbar bg-purple">
					<view class="action text-green">
						<view class="cuIcon-homefill"></view> 首页
					</view>
					<view class="action text-gray">
						<view class="cuIcon-similar"></view> 发现
					</view>
					<view class="action text-gray add-action">
						<button class="cu-btn cuIcon-add bg-green shadow"></button>
					</view>
					<view class="action text-gray">
						<view class="cuIcon-cart">
							<view class="cu-tag badge">99</view>
						</view>
						商城
					</view>
					<view class="action text-gray">
						<view class="cuIcon-my">
							<view class="cu-tag badge"></view>
						</view>
						我的
					</view>
				</view>
			</view>
				</view>
</template>

<script>
	export default {
		data() {
		return {
				PageCur: 'basics'
			}
		},
		methods: {
			NavChange: function(e) {
				this.PageCur = e.currentTarget.dataset.cur
			}
		}
	}
</script>

<style>
.box{
	width:100vw;
	
	
}
.bottom-wrapper{
	position:fixed;
	bottom:0px;
	
	
}
</style>
