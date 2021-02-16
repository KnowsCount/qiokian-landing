<!--
 * @Date: 16/02/2021 14.17.57 +0800
 * @Author: KnowsCount
 * @LastEditTime: 16/02/2021 15.35.49 +0800
 * @FilePath: /qiokian-landing/src/App.vue
-->
<template>
	<NavBar msg="Welcome to Your Vue.js App"/>
	<Content/>
</template>

<script>
import NavBar from './components/nav-bar'
import Content from './components/content'

export default {
	name: 'App',
	components: {
		NavBar,
		Content
	}
}
</script>

<style>
</style>
