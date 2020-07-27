<template>
	<view>
		登录页面
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
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

</style>
