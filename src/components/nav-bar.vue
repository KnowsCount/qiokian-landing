<!--
 * @Date: 16/02/2021 14.17.57 +0800
 * @Author: KnowsCount
 * @LastEditTime: 16/02/2021 15.36.41 +0800
 * @FilePath: /qiokian-landing/src/components/nav-bar.vue
-->
<template>
	<section>
		<header>
			<a href="#">
				<img class="logo" src="@/assets/logo.png">
			</a>
		<ul>
			<li><a href="#">Home</a></li>
			<li><a href="#">About</a></li>
			<li><a href="#">Demo</a></li>
		</ul>
		</header>
	</section>
</template>

<script>
export default {
	name: 'HelloWorld',
	props: {
		msg: String
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url(./app.css);
</style>
