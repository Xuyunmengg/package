<template>
	<view class="content">
		<view>
			<uni-grid :options='options' :show-border="false" @click='fn'></uni-grid>
		</view>
	</view>
</template>

<script>
	import uniGrid from "@/components/uni-grid/uni-grid.vue";
	export default {
		components: {
			uniGrid
		},
		data() {
			return {
				options: [{
						image: '../../static/img/kd.png',
						text: '寄快递'
					},
					{
						image: '../../static/img/gj.png',
						text: '果酱'
					},
					{
						image: '../../static/img/love.png',
						text: '我的亲友'
					},
					{
						image: '../../static/img/clover.png',
						text: '精灵书屋'
					},
					{
						image: '../../static/img/ox.png',
						text: '蓝犀牛搬家'
					},
					{
						image: '../../static/img/hs.png',
						text: '手机回收'
					},
					{
						image: '../../static/img/bg.png',
						text: '包裹大作战'
					},
					{
						image: '../../static/img/wj.png',
						text: '玩具租赁'
					},
					{
						image: '../../static/img/sm.png',
						text: '数码租赁'
					},
					{
						image: '../../static/img/nz.png',
						text: '女装租赁'
					}
				]
			}
		},
		onLoad() {

		},
		methods: {
			fn(e) {
				if (e.index == 0) {
					uni.navigateTo({
						url: '../first/jkd'
					});
				}
				if(e.index==1){
					uni.navigateTo({
						url: '../home/login'
					});
				}
			}
		}
	}
</script>

<style>

</style>
