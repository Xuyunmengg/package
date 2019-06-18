<template>
	<view class="content">
		<view>
			<input type="text" placeholder="请输入淘宝账户" v-model="username" />
			<input type="password" placeholder="请输入密码" v-model="password" />
			<button @click="register">同意协议并注册</button>
			<view>
				<span>已阅读并同意以下协议</span>
				<span class="treaty" @click="service">《淘宝服务协议》</span>，
				<span class="treaty" @click="hide">《隐私权政策》</span>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			service(){
				uni.navigateTo({
					url: 'service'
				});
			},
			hide(){
				uni.navigateTo({
					url: 'hide'
				});
			}
		}
	}
</script>

<style>
	@import url("../../static/css/login.css");
</style>
