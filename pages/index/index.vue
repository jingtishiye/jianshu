<template>
	<!-- <view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
	</view> -->
	<view><image src="../../static/wife.jpg" mode="widthFix"></view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			// #ifdef APP-PLUS
			uni.login({
			  provider: 'weixin',
			  success: function (loginRes) {
			    //console.log(loginRes.authResult);
				console.log(loginRes)
				console.log('---------------')
				console.log(JSON.stringify())
			  }
			});
			// #endif
		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
