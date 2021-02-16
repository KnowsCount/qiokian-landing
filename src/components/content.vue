<!--
 * @Date: 16/02/2021 15.35.09 +0800
 * @Author: KnowsCount
 * @LastEditTime: 16/02/2021 23.03.51 +0800
 * @FilePath: /qiokian-landing/src/components/content.vue
-->

<template>
	<section>
		<div class="content">
			<div class="textBox">
				<h2>🙊 live2d anime in vue.js:
					<br />
					<span>Qiokian!</span>
				</h2>
				<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
			</div>
			<div>
				<img class="logo" src="../assets/logo.png" />
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: 'Content',
}
</script>

<style>
@import url(./app.css);
.content {
	position: relative;
	width: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.content .textBox {
	position: relative;
	max-width: 700px;
}

.content .textBox h2 {
	position: relative;
	max-width: 700px;
	font-size: 4em;
	line-height: 1.4em;
	font-weight: 500;
}

.content .textBox h2 span {
	color: green;
	font-size: 1.2em;
	font-weight: 900;
}

.logo {
	max-width: 200px;
}

</style>