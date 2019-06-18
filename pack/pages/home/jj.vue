<template>
    <view>
        <uni-segmented-control :current="current" :values="items" @clickItem="onClickItem" style-type="button" active-color="#007aff"></uni-segmented-control>
        <view class="content">
            <view v-show="current === 0">
                <jijian1></jijian1>
            </view>
            <view v-show="current === 1">
                <jijian2></jijian2>
            </view>
            <view v-show="current === 2">
                选项卡3的内容
            </view>
        </view>
    </view>
</template>

<script>
	import uniSegmentedControl from "@/components/uni-segmented-control/uni-segmented-control.vue"
	import jijian1 from "../index/jijian1.vue"
	import jijian2 from "../index/jijian2.vue"
	export default {
	 components: {uniSegmentedControl,jijian1,jijian2},
		data() {
			return {
				items: ['速递寄件','驿站寄件','公益寄件'],
				current: 0
			}
		},
		methods: {
			onClickItem(index) {
				if (this.current !== index) {
					this.current = index;
				}
			}
		}
	}
</script>

<style>
	@import url("../../static/css/jj.css");
</style>
