<template>
	<view>
		<MyTest containerWidth="850" cWidth="650" cycleRadius="40" v-on:end="endfuntion" :password="password"></MyTest>
	</view>
</template>

<script>
	import MyTest from '../../components/mpvueGestureLock/index.vue';

	export default {
		components: {
			'MyTest': MyTest
		},
		data() {
			return {
				password: [1, 2, 3, 4, 5, 6, 7, 8, 9]
			};
		},
		methods: {
			endfuntion: function(e) {
				console.log(e)
			}
		}
	}
</script>

<style>
    body,
    page {
		padding: 0upx;
		margin: 0upx;
    }
</style>
