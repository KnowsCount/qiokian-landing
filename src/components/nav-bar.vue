<!--
 * @Date: 16/02/2021 14.17.57 +0800
 * @Author: KnowsCount
 * @LastEditTime: 17/02/2021 15.08.57 +0800
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
		<div class="circle"></div>
		<Content />
	</section>
</template>

<script>
import Content from './content'

export default {
	name: 'NavBar',
	props: {
		msg: String
	},
	components: {
		Content
	}
}
</script>

<style>
@import url(./app.css);
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

.circle {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: green;
	clip-path: circle(600px at right 800px);
}

</style>
