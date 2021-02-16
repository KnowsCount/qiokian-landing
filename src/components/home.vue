<!--
 * @Date: 16/02/2021 22.28.28 +0800
 * @Author: KnowsCount
 * @LastEditTime: 16/02/2021 22.58.24 +0800
 * @FilePath: /qiokian-landing/src/components/home.vue
-->

<template>
	<NavBar />
	<Content />
</template>

<script>
import NavBar from './nav-bar'
import Content from './content'

export default {
	components: {
		NavBar,
		Content
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
</style>