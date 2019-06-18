<template>
	<view>
		<view class="content">
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
	</view>
</template>

<script>
	import uniSwiperDot from "@/components/uni-swiper-dot/uni-swiper-dot.vue"
	export default {
		 components: {uniSwiperDot},
    data() {
        return {
            info: [{
                content: '../../static/imgs/lunbo1.png'
            }, {
                content: '../../static/imgs/lunbo2.png'
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
