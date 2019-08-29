<template>
	<div
		class="row"
		:style="{
			alignItems: align,
			justifyContent: justify,
			paddingTop: gutter.top,
			paddingBottom: gutter.bottom,
			width: width
		}"
	>
		<slot></slot>
	</div>
</template>

<script>
export default {
	props: {
		gutter: { // 上下边距
			type: Object,
			default() {
				return {
					top: "0",
					bottom: "0"
				};
			}
		},
		align: { //  垂直位置
			type: String,
			default: "top",
			validator: function(value) {
				return ["top", "middle", "bottom"].indexOf(value) >= 0;
			}
		},
		justify: { // 水平位置
			type: String,
			default: "start",
			validator: function(value) {
				return (
					["start", "end", "center", "space-around", "space-between"].indexOf(
						value
					) >= 0
				);
			}
		},
		width: { // 宽度
			type: String
		}
	}
};
</script>

<style lang="less" scoped>
.row {
	display: flex;
	flex-direction: row;
	justify-content: space-around;
	align-items: top;
}
</style>