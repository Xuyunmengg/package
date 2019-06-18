<template>
	<view class="content">
		
		<view>
			 <image class="sao" src="../../static/imgs/sys.png"></image>
			 <view class="sao1">扫一扫</view>
			 <view class="query">
				 <input type="text" placeholder="一键查全网包裹" />
			 </view>
			 <view>
				 <image class="news" src="../../static/imgs/xx.png"></image>
				 <view class="news1">消息</view>
			 </view>
			 <view>
				 <charts></charts>
			 </view>
			 <view>
				 <lattice></lattice>
			 </view>
			 <view class="yunshu1">运输中1</view>
			 <view class="t">
			 	<image class="bear" src="../../static/img/bear.jpg"></image>
			 	<view class="yunshu">运输中 预计明天到达</view>
			 	<view class="tmall">天猫 | 【xia】小熊加湿器</view>
			 	<view class="express">中通快递:漯河转周口</view>
			 </view>
			 
			 <view class="yunshu1">未发货1</view>
			 <view class="t">
			 	<image class="bear" src="../../static/img/ykc.jpg"></image>
			 	<view class="yunshu">未发货</view>
			 	<view class="tmall">天猫 | 【眼熟我了】遥控车</view>
			 	<view class="express">暂无物流信息</view>
			 </view>
			 
			 <view class="yunshu1">近日签收</view>
			 <view class="t">
			 	<image class="bear" src="../../static/img/tr.jpg"></image>
			 	<view class="yunshu">已签收</view>
			 	<view class="tmall">淘宝 | 【眼熟我了】身体乳</view>
			 	<view class="express">中通快递:周口已签收</view>
			 </view>
		</view>
		<view class="like">-猜你喜欢-</view>
		
			<view class="tb1">
				<image class="img1" src="../../static/img/tb1.jpg"></image>
				<view class="word">日系软妹遮阳伞可爱雨伞女折叠晴雨两用小清新防晒原宿卡通太阳伞</view>
				<view class="money">￥35.9</view>
			</view>
			<view class="tb2">
				<image class="img2" src="../../static/img/tb2.jpg"></image>
				<view class="word">zhuzhujia 发绳发饰头绳皮套头发橡皮筋女韩版可爱小恐龙韩国</view>
				<view class="money">￥12.9</view>
			</view>
		
		
			<view class="tb1">
				<image class="img1" src="../../static/img/tb1.jpg"></image>
				<view class="word">日系软妹遮阳伞可爱雨伞女折叠晴雨两用小清新防晒原宿卡通太阳伞</view>
				<view class="money">￥35.9</view>
			</view>
			<view class="tb2">
				<image class="img2" src="../../static/img/tb2.jpg"></image>
				<view class="word">zhuzhujia 发绳发饰头绳皮套头发橡皮筋女韩版可爱小恐龙韩国</view>
				<view class="money">￥12.9</view>
			</view>
		
			<view class="tb1">
				<image class="img1" src="../../static/img/tb1.jpg"></image>
				<view class="word">日系软妹遮阳伞可爱雨伞女折叠晴雨两用小清新防晒原宿卡通太阳伞</view>
				<view class="money">￥35.9</view>
			</view>
			<view class="tb2">
				<image class="img2" src="../../static/img/tb2.jpg"></image>
				<view class="word">zhuzhujia 发绳发饰头绳皮套头发橡皮筋女韩版可爱小恐龙韩国</view>
				<view class="money">￥12.9</view>
			</view>
			
	</view>
</template>

<script>
	import charts from "../index/charts.vue"
	import lattice from "../index/lattice.vue"
	export default {
		components: {charts,lattice},
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
	@import url("../../static/css/index.css");
	
</style>
