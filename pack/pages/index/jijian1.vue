<template>
		<view class="content">
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
			<view >
				<button class="buttons">下一步</button>
				<p class="p">守时守约  |   丟损必赔   |   速递官方保障</p>
			</view>
			<view>
				<image class="image" src="../../static/img/lunbo.jpg"></image>
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

		}
	}
</script>

<style>
	@import url("../../static/css/jj.css");
	
</style>
