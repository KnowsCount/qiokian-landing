<!--
 * @Date: 17/02/2021 20.55.08 +0800
 * @Author: KnowsCount
 * @LastEditTime: 17/02/2021 20.55.09 +0800
 * @FilePath: /qiokian-landing/src/components/qiokian.vue
-->

<template>
	<div></div>
</template>

<script>
/* eslint-disable */
export default {
	data() {
		return {
			live2d_path:
				'https://cdn.jsdelivr.net/gh/knowscount/live2d-widget@0.8.6/',
			cdnPath: 'https://cdn.jsdelivr.net/gh/fghrsh/live2d_api/',
		}
	},
	mounted() {
		this.__init()
	},
	methods: {
		__init() {
			this.loadAssets()
		},
		loadAssets() {
			// 加载 waifu.css live2d.min.js waifu-tips.js
			if (screen.width >= 768) {
				Promise.all([
					this.loadExternalResource(
						this.live2d_path + 'waifu.css',
						'css'
					),
					this.loadExternalResource(
						this.live2d_path + 'live2d.min.js',
						'js'
					),
					this.loadExternalResource(
						this.live2d_path + 'waifu-tips.js',
						'js'
					),
				]).then(() => {
					initWidget({
						waifuPath: this.live2d_path + 'waifu-tips.json',
						//apiPath: "https://live2d.fghrsh.net/api/",
						cdnPath: this.cdnPath,
					})
				})
			}
			// initWidget 第一个参数为 waifu-tips.json 的路径，第二个参数为 API 地址
			// API 后端可自行搭建，参考 https://github.com/fghrsh/live2d_api
			// 初始化看板娘会自动加载指定目录下的 waifu-tips.json
		},

		// 封装异步加载资源的方法
		loadExternalResource(url, type) {
			// 注意：live2d_path 参数应使用绝对路径
			// const live2d_path =
			//   "https://cdn.jsdelivr.net/gh/stevenjoezhang/live2d-widget@latest/";
			//const live2d_path = "/live2d-widget/";
			return new Promise((resolve, reject) => {
				let tag

				if (type === 'css') {
					tag = document.createElement('link')
					tag.rel = 'stylesheet'
					tag.href = url
				} else if (type === 'js') {
					tag = document.createElement('script')
					tag.src = url
				}
				if (tag) {
					tag.onload = () => resolve(url)
					tag.onerror = () => reject(url)
					document.head.appendChild(tag)
				}
			})
		},
	},
}
</script>

<style></style>
