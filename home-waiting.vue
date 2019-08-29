<template>
	<div class="home-waiting" v-show="isShow">
		<skeleton-loading>
			<!-- banner -->
			<row
				:gutter="{
					bottom: '15px'
				}"
			>
				<column :span="1">
					<rectangle
						:count="1"
						:boxProperties="{
							height: '144px',
							top: '14px'
						}"
					></rectangle>
				</column>
				<column :span="22">
					<rectangle
						:count="1"
						:boxProperties="{
							height: '172px'
						}"
					></rectangle>
				</column>
				<column :span="1">
					<rectangle
						:count="1"
						:boxProperties="{
							height: '144px',
							top: '14px'
						}"
					></rectangle>
				</column>
			</row>
			<!-- title -->
			<row align="middle">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- icon list -->
			<row :gutter="{ top: '20px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<row :gutter="{ top: '10px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<!-- title -->
			<row align="middle" :gutter="{ top: '20px' }">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- ad -->
			<row :gutter="{ top: '20px' }">
				<rectangle
					:boxProperties="{
						bottom: '10px',
						height: '100px'
					}"
				>
				</rectangle>
			</row>
			<!-- title -->
			<row align="middle" :gutter="{ top: '20px' }">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- activity -->
			<row :gutter="{ top: '20px' }">
				<rectangle
					:count="1"
					:boxProperties="{
						bottom: '10px',
						height: '172px'
					}"
				>
				</rectangle>
			</row>
			<row :gutter="{ top: '10px' }" width="80%">
				<rectangle
					:count="1"
					:boxProperties="{
						bottom: '10px',
						height: '30px'
					}"
				>
				</rectangle>
			</row>
			<row :gutter="{ top: '5px' }" justify="space-between">
				<rectangle
					:count="1"
					:boxProperties="{
						bottom: '10px',
						height: '20px',
						width: '40px'
					}"
				>
				</rectangle>
				<rectangle
					:count="1"
					:boxProperties="{
						bottom: '10px',
						height: '20px',
						width: '40px'
					}"
				>
				</rectangle>
			</row>
			<!-- title -->
			<row align="middle" :gutter="{ top: '20px' }">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- icon list -->
			<row :gutter="{ top: '20px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<row :gutter="{ top: '10px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<!-- ad2 -->
			<row :gutter="{ top: '20px' }">
				<rectangle
					:boxProperties="{
						bottom: '10px',
						height: '200px'
					}"
				>
				</rectangle>
			</row>
			<!-- app list2 -->
			<!-- title -->
			<row align="middle" :gutter="{ top: '20px' }">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- icon list -->
			<row :gutter="{ top: '20px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<!-- title -->
			<row align="middle" :gutter="{ top: '20px' }">
				<column :span="2">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="22" :gutter="10">
					<rectangle
						:boxProperties="{
							width: '100px',
							height: '28px'
						}"
					>
					</rectangle>
				</column>
			</row>
			<!-- icon list -->
			<row :gutter="{ top: '20px' }" justify="space-between">
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="5">
					<circle-skeleton></circle-skeleton>
				</column>
			</row>
			<!-- 资讯 -->
      <row :gutter="{ top: '20px' }">
				<rectangle
					:boxProperties="{
						bottom: '10px',
						height: '160px'
					}"
				>
				</rectangle>
			</row>
			<row v-for="index in 4" :key="index" align="middle" :gutter="{ top: '20px' }">
				<column :span="4">
					<circle-skeleton></circle-skeleton>
				</column>
				<column :span="20" :gutter="20">
					<rectangle
						:boxProperties="{
							top: '0px',
							width: 'auto',
							height: '20px'
						}"
					>
					</rectangle>
					<rectangle
						:boxProperties="{
							width: 'auto',
							height: '20px',
							top: '10px'
						}"
					>
					</rectangle>
				</column>
			</row>
		</skeleton-loading>
	</div>
</template>

<script>
import Row from "@/components-base/skeleton-loading/skeleton-row";
import Column from "@/components-base/skeleton-loading/skeleton-column";
import CircleSkeleton from "@/components-base/skeleton-loading/circle-skeleton";
import Rectangle from "@/components-base/skeleton-loading/rectangle-skeleton";
import SkeletonLoading from "@/components-base/skeleton-loading/skeleton-loading";
const COMPONENT_NAME = "home-waiting";

export default {
	name: COMPONENT_NAME,
	props: {
		isShow: {
			type: Boolean,
			default: false
		}
	},
	components: {
		Row,
		Column,
		CircleSkeleton,
		Rectangle,
		SkeletonLoading
	}
};
</script>

<style lang="less">
.home-waiting {
	padding: 20px;
}
</style>