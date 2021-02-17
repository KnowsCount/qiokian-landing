<!--
 * @Date: 16/02/2021 22.28.28 +0800
 * @Author: KnowsCount
 * @LastEditTime: 17/02/2021 20.55.40 +0800
 * @FilePath: /qiokian-landing/src/components/home.vue
-->

<template>
	<Qiokian />
	<NavBar />
</template>

<script>
import NavBar from './nav-bar'
import Qiokian from './qiokian'

export default {
	components: {
		NavBar,
		Qiokian
	}
}
</script>

<style>
* {
	font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
		Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	box-sizing: border-box;
	margin: 0;
	padding: 0;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}

section {
	position: relative;
	width: 100%;
	padding: 100px;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background: #fff;
}
</style>