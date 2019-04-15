<template>
	<view class="page">
		<view class="example-title">有底色</view>
		<view class="example-body">
			<uni-badge text="1"></uni-badge>
			<uni-badge text="2" type="primary"></uni-badge>
			<uni-badge text="34" type="success"></uni-badge>
			<uni-badge text="45" type="warning"></uni-badge>
			<uni-badge text="123" type="error"></uni-badge>
		</view>
		<view class="example-title">无底色</view>
		<view class="example-body">
			<uni-badge text="1" :inverted="true"></uni-badge>
			<uni-badge text="2" type="primary" :inverted="true"></uni-badge>
			<uni-badge text="34" type="success" :inverted="true"></uni-badge>
			<uni-badge text="45" type="warning" :inverted="true"></uni-badge>
			<uni-badge text="123" type="error" :inverted="true"></uni-badge>
		</view>
		<view class="example-title">迷你</view>
		<view class="example-body">
			<uni-badge text="1" size="small"></uni-badge>
			<uni-badge text="2" type="primary" size="small"></uni-badge>
			<uni-badge text="34" type="success" size="small"></uni-badge>
			<uni-badge text="45" type="warning" size="small"></uni-badge>
			<uni-badge text="123" type="error" size="small"></uni-badge>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {};
	}
};
</script>

<style>
.uni-badge {
	margin: 20upx;
}
</style>
