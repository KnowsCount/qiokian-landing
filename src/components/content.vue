<!--
 * @Date: 16/02/2021 15.35.09 +0800
 * @Author: KnowsCount
 * @LastEditTime: 17/02/2021 15.06.06 +0800
 * @FilePath: /qiokian-landing/src/components/content.vue
-->

<template>
	<div class="content">
		<div class="textBox">
			<h2>🙊 live2d anime in vue.js:
				<br />
				<span>Qiokian!</span>
			</h2>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
			<a href="#">Learn More</a>
		</div>
		<div class="imgBox">
			<!-- <img class="imgBox" src="../assets/shishiro_botan.png" /> -->
			<img class="shishiro" src="../assets/img1.png" />
		</div>
	</div>
	<ul class="thumb">
		<li>
			<img src="../assets/thumb1.png" alt="thumb-1">
		</li>
		<li>
			<img src="../assets/thumb2.png" alt="thumb-2">
		</li>
		<li>
			<img src="../assets/thumb3.png" alt="thumb-3">
		</li>
	</ul>
</template>

<script>
export default {
	name: 'Content',
}
</script>

<style scoped>
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
	max-width: 750px;
}

.content .textBox h2 {
	color: #333;
	position: relative;
	max-width: 750px;
	font-size: 3.5em;
	line-height: 1.4em;
	font-weight: 500;
}

.content .textBox h2 span {
	color: green;
	font-size: 1.2em;
	font-weight: 900;
}

.content .textBox p {
	color: #333;
}

.content .textBox a {
	text-decoration: none;
	display: inline-block;
	margin-top: 20px;
	padding: 8px 20px;
	background: green;
	color: #fff;
	border-radius: 40px;
	font-weight: 500;
	letter-spacing: 1px;
}

.content .imgBox {
	width: 600px;
	display: flex;
	justify-content: flex-end;
	padding-right: 50px;
	margin-top: 50px; 
}

.content .imgBox img {
	max-height: 580px;
}

.thumb {
	position: absolute;
	left: 50%;
	bottom: 20px;
	transform: translateX(-50%);
	display: flex;
}

.thumb li {
	list-style: none;
	display: inline-block;
	margin: 0 20px;
	cursor: pointer;
	transition: 0.5s;
}

.thumb li:hover {
	transform: translateY(-15px);
}

.thumb li img {
	max-width: 60px;
}

/* .logo {
	max-width: 400px;
} */

</style>