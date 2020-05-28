<template>
	<view class="content">
		<!-- 轮播图 -->
		<swiper indicator-dots circular autoplay>
			<swiper-item>
				<image src="../../static/1.jpg"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/2.jpg"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/3.jpg"></image>
			</swiper-item>
		</swiper>
		<!-- 导航区域 -->
		<view class="nav">
			<view class="nav_item">
				<view class="nav_item1">
					<image src="../../static/logo.png"></image>
				</view>
				<text>黑马超市</text>
			</view>
			<view class="nav_item">
				<view class="nav_item1"><image src="../../static/logo.png"></image></view>
				<text>联系我们</text>
			</view>
			<view class="nav_item">
				<view class="nav_item1"><image src="../../static/logo.png"></image></view>
				<text>社区图片</text>
			</view>
			<view class="nav_item">
				<view class="nav_item1"><image src="../../static/logo.png"></image></view>
				<text>学习视频</text>
			</view>
		</view>
		
		<!-- 推荐商品 -->
		<view class="hot_goods">
			<view class="title">推荐商品</view>
			
			<!-- 商品列表 -->
			<view class="goods_list">
				<view class="goods_item">
					<image src="../../static/5.jpg"></image>
					<text></text>
					<text></text>
					<view></view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	// import uniSwiperDot from "@/components/uni-swiper-dot/uni-swiper-dot.vue"
	export default {
		name:"index",
		components:{
			// uniSwiperDot
		},
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content{
		swiper{
			width: 750rpx;
			height: 380rpx;
			image{
				height: 100%;
				width: 100%;
			}
		}
		.nav {
			display: flex;
			.nav_item {
				width: 25%;
				text-align: center;
				.nav_item1 {
					width: 120rpx;
					height: 120rpx;
					background: $shop-color;
					margin: 10px auto;
					border-radius: 60rpx;
					line-height: 120rpx;
					image{
						width: 50rpx;
						height: 50rpx;
					}
					text{
						font-size: 30rpx;
					}
				}
			}
	    }
		.hot_goods {
			background: #eee;
			overflow: hidden;
			margin-top: 5rpx;
			.title {
				width: 750rpx;
				height: 50px;
				line-height: 50px;
				text-align: center;
				background: #FFFFFF;
				margin: 8rpx auto;
				letter-spacing: 20rpx;
				color: $shop-color;
			}
		}
		.goods_list{
			padding: 0 10rpx;
			.goods_item {
				width: 360rpx;
				background: #FFFFFF;
				image {
					width: 100%;
				}
			}
		}
	}
</style>
