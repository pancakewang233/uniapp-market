<template>
	<view>
		<!-- 顶部导航栏 -->
		<u-navbar
			title=""
			bgColor="40AE36"
		>
			<template #left>
				<view>
					左边
				</view>
			</template>
			<template #right>
				<view>
					右边
				</view>
			</template>
		</u-navbar>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {
			trigger(){
				console.log('----waht here fucking ----')
			}
		}
	}
</script>

<style>
</style>
