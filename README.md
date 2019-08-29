# skeleton
骨架屏组件实现

## 核心组件
<template>
	<div class="skeleton-loading">
		<div class="skeleton-bac-animation"></div>
		<slot></slot>
	</div>
</template>

<script>
export default {}
</script>

<style lang="less" scoped>
.skeleton-loading {
	position: relative;
	width: 100%;
	@keyframes backpos {
		from {
			background-position-x: -200px;
		}
		to {
			background-position-x: calc(200px + 100%);
		}
	}
	.skeleton-bac-animation {
		position: absolute;
		z-index: auto;
		width: 100%;
		height: 100%;
		background: linear-gradient(
			to right,
			rgba(255, 255, 255, 0),
			rgba(255, 255, 255, 0.5) 50%,
			rgba(255, 255, 255, 0) 80%
		);
		background-size: 30% 100%;
		background-repeat: no-repeat;
		animation: backpos 1s ease-in-out 0s infinite;
	}
}
</style>
