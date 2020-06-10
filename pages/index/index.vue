<template>
	<view class="content">
		<view class="header">
			<image class="banner-bg" src="../../static/banner-bg.jpg"></image>
			<view class="header-container">
				<view class="search-bar">
					<icon class="iconfont icon-category"></icon>
					<view class="input-area">
						<image class="jd-logo" src="../../static/images/jd-logo.png"></image>
						<u-input placeholder="怡宝矿泉水"></u-input>
					</view>
					<text class="login-btn">登录</text>
				</view>
				<view class="swiper-container">
					<u-swiper :list="swiperDataSource"></u-swiper>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				swiperDataSource: [{
					image: '/static/index-banner1.jpg'
				}, {
					image: '/static/index-banner2.jpg'
				}, {
					image: '/static/index-banner3.jpg'
				}]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		background-color: #f6f6f6;
	}
	.header {
		position: relative;
	}
	.banner-bg {
		width: 100%;
	}
	.header-container {
		position: absolute;
		width: 100%;
		top: 0;
	}
	.search-bar {
		display: flex;
		align-items: center;
	}
	.input-area {
		flex-grow: 1;
		background-color: white;
		border-radius: 10000rpx;
		height: 48rpx;
		display: flex;
		align-items: center;
		padding: 4rpx 24rpx;
	}
	.jd-logo {
		height: 28rpx;
		width: 28rpx;
	}
	.icon-category {
		font-size: 48rpx;
	}
	.login-btn, .icon-category {
		color: white;
		padding: 22rpx;
	}
	.swiper-container {
		margin: 0 22rpx;
	}
</style>
