<!--
 * @Date: 16/02/2021 22.28.28 +0800
 * @Author: KnowsCount
 * @LastEditTime: 17/02/2021 22.17.03 +0800
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

@media ( max-width: 991px ) {
	header {
		padding: 20px;
	}

	header .logo {
		max-width: 60px;
	}

	.toggle {
		position: relative;
		width: 30px;
		height: 30px;
		cursor: pointer;
		background: url(../assets/menu.png);
		background-size: 30px;
		background-position: center;
		background-repeat: no-repeat;
		filter: invert(1);
		z-index: 11;
	}

	.toggle.active {
		background: url(../assets/close.png);
		background-size: 30px;
		background-position: center;
		background-repeat: no-repeat;
	}

	header ul {
		display: none;
	}

	header ul li a {
		display: inline-block;
		font-size: 1.5em;
		font-weight: 400;
		margin: 5px 0;
		text-decoration: none;
	}

	header ul.navigation.active {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		background: #fff;
		z-index: 10;
	}

	section {
		padding: 20px 20px 120px;
	}

	.content {
		flex-direction: column;
		margin-top: 100px;
	}

	.content .textBox {
		max-width: 100%;
	}

	.content .imgBox {
		max-width: 100%;
	}

	.content .imgBox img {
		max-width: 300px;
	}
	
	.content .textBox h2 {
		font-size: 2.5em;
		margin-bottom: 15px;
	}

	.circle {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: green;
		clip-path: circle(400px at center bottom);
	}

	.thumb li img {
		max-width: 40px;
	}
}
</style>