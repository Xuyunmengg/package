<template>
	<view class="content">
		<view>
			<button @click="fn">
				<span class="buttons2">智能录入地址</span>
				<span class="buttons3">帮您识别图片或文本中的信息</span>
			</button>
		</view>
		<view>
			<image class="jkd" src="../../static/image/ji.png"></image>
			<view class="bor">
				<input class="input" type="text" placeholder="请输入寄件人及地址" />
			</view>
		</view>
		<view>
			<image class="shou" src="../../static/image/shou.png"></image>
			<view class="bor">
				<input class="input" type="text" placeholder="请输入收件人及地址" />
			</view>
		</view>
		<view>
			<button class="buttons">下单</button>
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
			fn(){
				uni.navigateTo({
					url: ''
				});
			
			},
		}
	}
</script>

<style>

	@import url("../../static/css/jj.css");
</style>
