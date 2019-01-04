<template>
	<view>
		<view class="uni-flex uni-row">
			<view class="text" style="width: 80upx;height: 80upx;display: flex; justify-content: center;align-items: center;">
				<image src="../../../static/tips.png" style="width: 80upx;height: 80upx;"></image>
			</view>
			<view class="uni-flex uni-column" style="flex: 1;justify-content: space-between;">
				<view class="uni-flex uni-row" style="height: 40upx; justify-content: space-between;">
					<view class="text" style="flex-shrink: 1; font-weight: bold; align-items: center;">1111111111</view>
					<view class="text" style="flex-shrink: 0; font-size: 10px; text-align: right; align-items: center; color: grey;">0/1完成</view>
				</view>
				<view class="text" style="text-align: left; font-size: 10px; align-items: center; color: grey;">
					222222222222222222222
				</view>
			</view>
		</view>
		<view class="uni-flex uni-row">
			<view class="text" style="width: 80upx;height: 80upx;display: flex; justify-content: center;align-items: center;">
				<image src="../../../static/tips.png" style="width: 80upx;height: 80upx;"></image>
			</view>
			<view class="uni-flex uni-column" style="flex: 1;justify-content: space-between;">
				<view class="uni-flex uni-row" style="height: 40upx; justify-content: space-between;">
					<view class="text" style="flex-shrink: 1; font-weight: bold; align-items: center;">1111111111</view>
					<view class="text" style="flex-shrink: 0; font-size: 10px; text-align: right; align-items: center; color: grey;">0/1完成</view>
				</view>
				<view class="text" style="text-align: left; font-size: 10px; align-items: center; color: grey;">
					222222222222222222222
				</view>
			</view>
		</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				lists: [
				]
			}
		},
		onLoad() {
		},
		onShareAppMessage() {
			return {
			
			}
		},
		onNavigationBarButtonTap(e) {
			
		},
		methods: {
		}
	}
</script>

<style>
	page{
		height: auto;
		min-height: 100%;
		font-size: 12px;
	}
</style>
