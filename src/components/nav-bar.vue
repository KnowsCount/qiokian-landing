<!--
 * @Date: 16/02/2021 14.17.57 +0800
 * @Author: KnowsCount
 * @LastEditTime: 16/02/2021 23.01.18 +0800
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
	name: 'NavBar',
	props: {
		msg: String
	}
}
</script>

<style>
@import url(./app.css);
section {
	position: relative;
	width: 100%;
	padding: 50px;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background: #fff;
}

header {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	padding: 20px 100px;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

header .logo {
	position: relative;
	max-width: 80px;
}

header ul {
	position: relative;
	display: flex;
}

header ul li {
	list-style: none;
}

header ul li a {
	color: #333;
	display: inline-block;
	font-weight: 400;
	margin-left: 40px;
	text-decoration: none;
}
</style>
