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
		<view class="kuaidi">
			 <input type="text" placeholder="快递选择"/>
			 <input type="text" placeholder="上门时间"/>
			 <input type="text" placeholder="物品类型"/>
			 <input type="text" placeholder="保价"/>
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
	@import url("../../static/css/jkd.css");
</style>
