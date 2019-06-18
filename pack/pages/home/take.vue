<template>
	<view class="content">
		<view class="take">
			<image class="empty" src="../../static/img/empty.png"></image>
			<view class="null">没有包裹可以取哦</view>
		</view>
		<view class="history">历史包裹</view>
		<view class="t">
			<image class="sdz" src="../../static/img/sdz.jpg"></image>
			<view class="sign">已签收</view>
			<view class="Steward">淘宝 | 史迪仔泡泡机史迪奇</view>
			<view class="express">韵达快递:【周口市】被驿站签收</view>
		</view>
		<view class="t">
			<image class="sdz" src="../../static/img/sdz.jpg"></image>
			<view class="sign">已签收</view>
			<view class="Steward">淘宝 | 史迪仔泡泡机史迪奇</view>
			<view class="express">韵达快递:【周口市】被驿站签收</view>
		</view>
		<view class="t">
			<image class="sdz" src="../../static/img/sdz.jpg"></image>
			<view class="sign">已签收</view>
			<view class="Steward">淘宝 | 史迪仔泡泡机史迪奇</view>
			<view class="express">韵达快递:【周口市】被驿站签收</view>
		</view>
		<!-- 轮播图 -->
		
		<uni-swiper-dot :info="info" :current="current" field="content" :mode="mode">
			<swiper class="swiper-box" @change="change">
				<swiper-item v-for="(item ,index) in info" :key="index">
					<view class="swiper-item">
						<image :src="item.content" mode=""></image>
					</view>
				</swiper-item>
			</swiper>
		</uni-swiper-dot>
		
	</view>
</template>

<script>
	import uniSwiperDot from "@/components/uni-swiper-dot/uni-swiper-dot.vue"
	export default {
		 components: {uniSwiperDot},
    data() {
        return {
             info: [{
                content: '../../static/image/lunbo1.jpg'
            }, {
                content: '../../static/image/lunbo2.jpg'
            }, {
                content: '../../static/image/lunbo3.jpg'
            }],
            current: 0,
            mode: 'long',
        }
    },
    methods: {
        change(e) {
            this.current = e.detail.current;
        }
    }
}
</script>

<style>
	@import url("../../static/css/take.css");
	.swiper-item,image{
		width: 100%;
		height: 200upx;
	}
	.swiper-box{
		width: 100%;
		height: 200upx;
	}
	.content{
		margin-top: 20upx;
	}
</style>
