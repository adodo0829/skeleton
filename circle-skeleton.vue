<template>
<!-- 圆形样式 -->
	<div
		class="circle"
		ref="circle"
		:style="{
			backgroundColor: backColor,
			width: diameter,
			height: height
		}"
	></div>
</template>

<script>
export default {
	data() {
		return {
			height: 0
		};
	},
	props: {
		backColor: {
			type: String,
			default: "#e7e7e7"
		},
		diameter: {
			type: String,
			default: "100%"
		}
	},
	updated() {
		this.height = window.getComputedStyle(this.$refs.circle).width;
	},
	mounted() {
		this.height = window.getComputedStyle(this.$refs.circle).width;
	}
};
</script>

<style lang="less" scoped>
.circle {
	border-radius: 23%;
}
</style>

