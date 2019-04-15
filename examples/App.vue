<script>
export default {
	onLaunch: function() {
		console.log('App Launch');
	},
	onShow: function() {
		console.log('App Show');
	},
	onHide: function() {
		console.log('App Hide');
	}
};
</script>

<style lang="scss">
/*每个页面公共css */
page {
	display: flex;
	flex-direction: column;
	box-sizing: border-box;
	background-color: #f5f5f5;
}
view {
	font-size: $uni-font-size-base;
	line-height: inherit;
}
.example {
	padding: 0 30upx 30upx;
}
.example-title {
	font-size: $uni-font-size-lg;
	// line-height: $uni-font-size-base;
	color: $uni-text-color;
	padding: 30upx;
	margin-top: 20upx;
	position: relative;
	background-color: #fff;
}
.example-title__after {
	position: relative;
	color: #031e3c;
}
.example-title:after {
	content: '';
	position: absolute;
	left: 0;
	margin: auto;
	top: 0;
	bottom: 0;
	width: 6upx;
	height: 40upx;
	border-top-right-radius: 100upx;
	border-bottom-right-radius: 100upx;
	background-color: #031e3c;
}
.example .example-title {
	margin: 40upx 0;
}
.example-body {
	// padding: 0 40upx;
	border-top: 1px #f5f5f5 solid;
	padding: 30upx;
	background: #ffffff;
}
</style>
