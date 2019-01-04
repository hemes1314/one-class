<template>
	<view class="page">
		<view class="uni-list">
			<view class="uni-list-cell" hover-class="uni-list-cell-hover">
				<view class="uni-media-list">
					<view class="uni-media-list-logo">
						<image src="../../../static/user.png"></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">聆风 班主任</view>
						<view class="uni-media-list-text-bottom uni-ellipsis">莲葩园幼儿园19届01班</view>
					</view>
				</view>
			</view>
		</view>
		
		<view class="uni-list" style="margin-top: 20px;">
			<view class="uni-list-cell" hover-class="uni-list-cell-hover" v-for="(value,key) in list" :key="key">
				<view class="uni-media-list">
					<view class="uni-media-list-logo">
						<image v-if="showImg" :src="value.img"></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">{{value.title}}</view>
					</view>
				</view>
			</view>
		</view>
		
		<view class="uni-list" style="margin-top: 20px;">
			<view class="uni-list-cell" hover-class="uni-list-cell-hover">
				<view class="uni-media-list">
					<view class="uni-media-list-logo">
						<image src="../../../static/user.png" style=""></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">切换账号</view>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				title: 'media-list',
				showImg: false,
				list: [{
						title: "幸福",
						content: "能和心爱的人一起睡觉，是件幸福的事情；可是，打呼噜怎么办？",
						img: "https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/shuijiao.jpg?imageView2/3/w/200/h/100/q/90"
					},
					{
						title: "木屋",
						content: "想要这样一间小木屋，夏天挫冰吃瓜，冬天围炉取暖。",
						img: "https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/muwu.jpg?imageView2/3/w/200/h/100/q/90"
					},
					{
						title: "CBD",
						content: "烤炉模式的城，到黄昏，如同打翻的调色盘一般。",
						img: "https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/cbd.jpg?imageView2/3/w/200/h/100/q/90"
					}
				]
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
.title {
	padding: 20upx;
}
</style>
