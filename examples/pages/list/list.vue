<template>
	<view>
		<view class="example-title">基础列表</view>
		<uni-list>
			<uni-list-item title="列表文字" :show-arrow="false"></uni-list-item>
			<uni-list-item title="列表文字" note="列表描述信息" :show-arrow="false"></uni-list-item>
			<uni-list-item title="列表禁用状态" :disabled="true" :show-arrow="false"></uni-list-item>
		</uni-list>
		<view class="example-title">菜单列表</view>
		<uni-list>
			<uni-list-item title="列表右侧带箭头"></uni-list-item>
			<uni-list-item title="列表右侧带箭头 + 角标" :show-badge="true" badge-text="12"></uni-list-item>
			<uni-list-item title="列表左侧带略缩图" thumb="https://img-cdn-qiniu.dcloud.net.cn/new-page/uni.png"></uni-list-item>
			<uni-list-item title="列表左侧带扩展图标" :show-extra-icon="true" :extra-icon="extraIcon1"></uni-list-item>
			<uni-list-item title="列表右侧带 switch" :show-extra-icon="true" :extra-icon="extraIcon1" :show-switch="true" @switchChange="switchChange"></uni-list-item>
			<uni-list-item
				title="禁用状态"
				:disabled="true"
				:show-extra-icon="true"
				:extra-icon="extraIcon2"
				:show-switch="true"
				:switch-checked="true"
				@switchChange="switchChange"
			></uni-list-item>
		</uni-list>
		
	</view>
</template>

<script>
export default {
	data() {
		return {
			extraIcon1: {
				color: '#007aff',
				size: '22',
				type: 'gear-filled'
			},
			extraIcon2: {
				color: '#4cd964',
				size: '22',
				type: 'image'
			}
		};
	},
	methods: {
		switchChange(e) {
			uni.showToast({
				title: 'change:' + e.value,
				icon: 'none'
			});
		}
	}
};
</script>

<style></style>
