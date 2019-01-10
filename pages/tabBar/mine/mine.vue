<template>
	<view class="center">
		
		<!-- <view class="logo" @click="goLogin" :hover-class="!login ? 'logo-hover' : ''">
			<image class="logo-img" :src="login ? uerInfo.avatarUrl :avatarUrl"></image>
			<view class="logo-title">
				<text class="uer-name">Hi，{{login ? uerInfo.name : '您未登录'}}</text>
				<text class="go-login navigat-arrow" v-if="!login">&#xe6da;</text>
			</view>
		</view> -->
		<view class="uni-list">
			<view class="uni-list-cell" hover-class="uni-list-cell-hover">
				<view class="uni-media-list">
					<view class="uni-media-list-logo">
						<image v-if="showImg" :src="avatarUrl"></image>
					</view>
					<view class="uni-media-list-body">
						<view class="uni-media-list-text-top">聆风 班主任</view>
						<view class="uni-media-list-text-bottom uni-ellipsis">莲葩园 幼儿园19届01班</view>
					</view>
				</view>
			</view>
		</view>
	
		<view class="center-list">
			<view class="center-list-item border-bottom">
				<text class="list-icon" style="color: #D5CC39;">&#xe68c;</text>
				<text class="list-text">组建班级</text>
				<text class="navigat-arrow">&#xe6da;</text>
			</view>
			<view class="center-list-item border-bottom">
				<text class="list-icon" style="color: #DB973E;">&#xe600;</text>
				<text class="list-text">成员管理</text>
				<text class="navigat-arrow">&#xe6da;</text>
			</view>
			<view class="center-list-item">
				<text class="list-icon" style="color: #4986D8;">&#xe715;</text>
				<text class="list-text">帮助中心</text>
				<text class="navigat-arrow">&#xe6da;</text>
			</view>
		</view>
		<view class="center-list">
			<view class="center-list-item">
				<text class="list-icon" style="color: #07CD3E;">&#xe601;</text>
				<text class="list-text">切换账号</text>
				<text class="navigat-arrow">&#xe6da;</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				login: false,
				avatarUrl: "../../../static/user.png",
				uerInfo: {},
				showImg: false
			}
		},
		methods: {
			goLogin() {
				if (!this.login) {
					console.log("点击前往登录")
				}
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
	@font-face {
		font-family: 'iconfont';
		/* project id 1001933 */
		src: url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.eot');
		src: url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.eot?#iefix') format('embedded-opentype'),
			url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.woff2') format('woff2'),
			url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.woff') format('woff'),
			url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.ttf') format('truetype'),
			url('//at.alicdn.com/t/font_1001933_rdg55wjeo2b.svg#iconfont') format('svg');
	}

	page,
	view {
		display: flex;
	}

	.center {
		flex-direction: column;
	}

	.center-list {
		background-color: #FFFFFF;
		margin-top: 20upx;
		width: 750upx;
		flex-direction: column;
	}

	.center-list-item {
		height: 80upx;
		width: 750upx;
		box-sizing: border-box;
		flex-direction: row;
		padding: 0upx 20upx;
	}

	.border-bottom {
		border-bottom-width: 1upx;
		border-color: #c8c7cc;
		border-bottom-style: solid;
	}

	.list-icon {
		line-height: 80upx;
		font-size: 34upx;
		text-align: center;
		font-family: iconfont;
		margin-right: 20upx;
	}

	.list-text {
		line-height: 80upx;
		font-size: 25upx;
		font-weight: bold;
		color: #555;
		flex: 1;
		text-align: left;
	}

	.navigat-arrow {
		line-height: 80upx;
		font-size: 34upx;
		color: #555;
		text-align: right;
		font-family: iconfont;
	}
</style>
