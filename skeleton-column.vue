<template>
<!-- 列数 -->
	<div
		class="col"
		:style="{
			order: order,
			width: perWidth,
			padding: gutterToPadding
		}"
	>
		<slot></slot>
	</div>
</template>

<script>
export default {
	props: {
		gutter: { //左右的外边距
			type: Number,
			default: 0
		},
		span: { // 等分 24 份
			type: Number,
			required: true,
			validator: function(value) {
				return value <= 24;
			}
		},
		order: { // 优先级展示
			type: Number
		}
	},
	computed: {
		perWidth() {
			return ((this.span * 100) / 24).toFixed(2) + "%";
		},
		gutterToPadding() {
			return `0 ${this.gutter}px`;
		}
	}
};
</script>

<style lang="less">
</style>