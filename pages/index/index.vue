<template>
	<view>
		<!-- 顶部导航栏 -->
		<u-navbar title="" bgColor="40AE36">
			<template #left>
				<view class="left">
					<view>
						<u-icon name="map" color="#fff" size="24px"></u-icon>
					</view>
					<view style="margin-left: 16rpx; margin-right: 8rpx;">海淀区中关村大厦</view>
					<view>
						<u-icon name="arrow-down-fill" color="#fff" size="24px"></u-icon>
					</view>
				</view>
			</template>
			<template #right>
				<view class="right">
					<view>
						<u-icon name="scan" color="#fff" size="24px"></u-icon>
					</view>
					<view style="margin-left: 16rpx;">
						<u-icon name="chat" color="#fff" size="24px"></u-icon>
					</view>
				</view>
			</template>
		</u-navbar>
		<!-- 搜索区域 -->
		<view class="search">
			<u-search placeholder="日照香炉生紫烟" :show-action="false" :disabled="true" @click="onSearch"></u-search>
		</view>
		<!-- 轮播区 -->
		<view class="swiper">
			<u-swiper :list="list1"></u-swiper>
		</view>
		<!-- 金刚区 -->
		<view class="vajra">
			<u-row justify="space-between" gutter="10">
				<u-col span="2.4">
					<view class="demo-layout">
						<view class="img">
							<image src="../../static/logo.png" mode=""></image>
						</view>
						<view class="text">水果蔬菜</view>
					</view>
				</u-col>
				<u-col span="2.4">
					<view class="demo-layout">
						<view class="img">
							<image src="../../static/logo.png" mode=""></image>
						</view>
						<view class="text">肉禽蛋品</view>
					</view>
				</u-col>
				<u-col span="2.4">
					<view class="demo-layout">
						<view class="img">
							<image src="../../static/logo.png" mode=""></image>
						</view>
						<view class="text">海鲜水产</view>
					</view>
				</u-col>
				<u-col span="2.4">
					<view class="demo-layout">
						<view class="img">
							<image src="../../static/logo.png" mode=""></image>
						</view>
						<view class="text">速食冷冻</view>
					</view>
				</u-col>
				<u-col span="2.4">
					<view class="demo-layout">
						<view class="img">
							<image src="../../static/logo.png" mode=""></image>
						</view>
						<view class="text">粮油米面</view>
					</view>
				</u-col>
			</u-row>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list1: [
					'https://cdn.uviewui.com/uview/swiper/swiper1.png',
					'https://cdn.uviewui.com/uview/swiper/swiper2.png',
					'https://cdn.uviewui.com/uview/swiper/swiper3.png',
				]
			}
		},
		onLoad() {

		},
		methods: {
			trigger() {
				console.log('----waht here trigger ----')
			},
			onSearch() {
				console.log('----waht here onSearch ----')
			}
		}
	}
</script>

<style lang="scss">
	.left {
		display: flex;
		align-items: center;
		color: #fff;
		font-size: 30rpx;
	}

	.right {
		display: flex;
	}

	.search {
		margin-top: 44px;
		padding: 16rpx 26rpx;
	}

	.vajra{
		padding: 10rpx 24rpx;
	}
	
	.demo-layout {
		height: 25px;
		border-radius: 4px;
		flex-direction: column;
		align-items: center;
		.img{
			height: 108rpx;
			width: 108rpx;
			background-color: red;
			border-radius: 50%;
			margin-bottom: 6rpx;
			image{
				width: 100%;
				height: 100%;
				border-radius: 50%;
			}
		}
		.text{
			font-size: 24rpx;
			color: #666666;
		}
	}

</style>
