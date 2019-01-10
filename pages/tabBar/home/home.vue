<template>
	<view>
		<view class="uni-list">
			<view class="uni-list-cell" hover-class="uni-list-cell-hover">
				<view class="uni-media-list">
					<view class="uni-media-list-logo">
						<image v-if="showImg" :src="img_src"></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">111</view>
						<view class="uni-media-list-text-top-right">1/2</view>
						<view class="uni-media-list-text-bottom uni-ellipsis">222222</view>
					</view>
				</view>
			</view>
			<view class="uni-list-cell" hover-class="uni-list-cell-hover">
				<view class="uni-list-cell-navigate">
					<view class="uni-media-list-logo">
						<image v-if="showImg" :src="img_src"></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">111</view>
						<view class="uni-media-list-text-top-right">1/2</view>
						<view class="uni-media-list-text-bottom uni-ellipsis">222222</view>
					</view>
				</view>
			</view>
		</view>
		<view>
			<view class="uni-media-list-text-bottom-right">
				<image style="width: 100upx; height: 100upx;" src="../../../static/add.png"></image>
			</view>
		</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				img_src: "/static/tips.png",
				showImg: false
			}
		},
		onLoad() {
			setTimeout(() => {
				this.showImg = true;
			}, 400)
		}
	}
</script>

<style>
	uni-image {
		width: 80%;
		height: 80%;
	}
	.uni-media-list-text-top-right {
		font-family: uniicons;
		content: '1/2';
		position: absolute;
		right: 11px;
		top: 30%;
		color: #bbb;
		-webkit-transform: translateY(-50%);
		-ms-transform: translateY(-50%);
		transform: translateY(-50%);
	}
	.uni-media-list-text-bottom-right {
		position: absolute;
		right: 11px;
		bottom: 0%;
	}
</style>
