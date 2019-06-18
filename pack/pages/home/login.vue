<template>
	<view class="content">
		<view>
			<image class="logo" src="../../static/imgs/tb.png"></image>
		</view>
		<view>
			<input type="text" placeholder="请输入淘宝账户" v-model="username" />
			<view>
				<input type="password" placeholder="请输入密码" v-model="password" />
			</view>
			<button @click="login">登录</button>
			<view>
				<span class="pa">找回密码</span>
				<span class="re" @click="register">注册</span>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				username: '',
				password: '',
			
			};
		},
		mounted() {

		},
		methods: {
			
			register(){
				uni.navigateTo({
					url: 'register'
				});

			},
			login() {
				if(this.username.length<=0){
					uni.showToast({
						icon:'none',
						title:'用户名不能为空',
						
					});
					return;
				}
				if(this.password.length<=0){
					uni.showToast({
						icon:'none',
						title:'密码不能为空',
						
					});
					return;
				}
				
				uni.navigateTo({
					url: 'index'
				});
			}
		}
	}
</script>

<style>
	@import url("../../static/css/login.css");
</style>
