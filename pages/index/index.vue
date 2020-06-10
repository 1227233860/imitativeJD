<template>
	<view class="content">
		<view class="header-container">
			<view class="search-bar">
				<icon class="iconfont icon-category"></icon>
				<view class="input-area">
					<image class="jd-logo" src="../../static/images/jd-logo.png"></image>
					<u-line direction="col" />
					<u-icon class="icon-search" name="search"></u-icon>
					<u-input placeholder="怡宝矿泉水" :customStyle="{fontSize: '20rpx'}" placeholderStyle="color: #aaa"></u-input>
				</view>
				<text class="login-btn">登录</text>
			</view>
			<view class="swiper-container">
				<u-swiper :list="swiperDataSource"></u-swiper>
			</view>
		</view>
		<view>
			<view class="view-pager">
				<view>
					<image src="../../static/images/index-menu1.png"></image>
					<text>京东超市</text>
				</view>
				<view>
					<image src="../../static/images/index-menu2.png"></image>
					<text>数码电器</text>
				</view>
				<view>
					<image src="../../static/images/index-menu3.png"></image>
					<text>京东服饰</text>
				</view>
				<view>
					<image src="../../static/images/index-menu4.png"></image>
					<text>京东生鲜</text>
				</view>
				<view>
					<image src="../../static/images/index-menu5.png"></image>
					<text>京东到家</text>
				</view>
				<view>
					<image src="../../static/images/index-menu6.png"></image>
					<text>充值缴费</text>
				</view>
				<view>
					<image src="../../static/images/index-menu7.png"></image>
					<text>9.9拼购</text>
				</view>
				<view>
					<image src="../../static/images/index-menu8.png"></image>
					<text>领券</text>
				</view>
				<view>
					<image src="../../static/images/index-menu9.png"></image>
					<text>借钱</text>
				</view>
				<view>
					<image src="../../static/images/index-menu10.png"></image>
					<text>PLUS会员</text>
				</view>
			</view>
		</view>
		<view class="seckill">
			<image class="index-activity" src="../../static/images/index-activity.png"></image>
			<view class="seckill-container">
				<view class="seckill-title">
					<view>
						<text>京东秒杀</text>
						<view class="countdown">
							<text>18点场</text>
							<text>00:00:00</text>
						</view>
					</view>
					<text class="more-seckill">更多秒杀</text>
					<image class="more-seckill-icon" src="../../static/images/more-seckill.png"></image>
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
					image: '/static/images/index-banner1.jpg'
				}, {
					image: '/static/images/index-banner2.jpg'
				}, {
					image: '/static/images/index-banner3.jpg'
				}]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	@import 'index.scss';
</style>
