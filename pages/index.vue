<template>
	<section class="container">
		<div>
			<app-logo/>
			<h1 class="title">
				nuxt-study
			</h1>
		</div>
	</section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
	components: {
		AppLogo
	}
}
</script>

<style>
.container {
	min-height: 100vh;
}

.title {
	font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
	display: inline;
	font-weight: 300;
	font-size: 40px;
	color: #35495e;
	letter-spacing: 1px;
}
</style>
