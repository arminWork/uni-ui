<template>
	<view>
		<view class="example-title">一般用法</view>
		<view class="example-body"><uni-countdown :day="1" :hour="1" :minute="12" :second="40"></uni-countdown></view>
		<view class="example-title">不显示天数</view>
		<view class="example-body"><uni-countdown :show-day="false" :hour="12" :minute="12" :second="12"></uni-countdown></view>
		<view class="example-title">文字分隔符</view>
		<view class="example-body"><uni-countdown :minute="30" :second="0" :show-colon="false"></uni-countdown></view>
		<view class="example-title">修改颜色</view>
		<view class="example-body">
			<uni-countdown color="#FFFFFF" background-color="#00B26A" border-color="#00B26A" :day="1" :hour="2" :minute="30" :second="0"></uni-countdown>
		</view>
		<view class="example-title">倒计时回调事件</view>
		<view class="example-body"><uni-countdown :show-day="false" :second="10" @timeup="timeup"></uni-countdown></view>
	</view>
</template>
<script>
export default {
	data() {
		return {};
	},
	methods: {
		timeup() {
			uni.showToast({
				title: '时间到'
			});
		}
	}
};
</script>

<style>
.title {
	margin: 80upx 0 20upx 0;
}
</style>
