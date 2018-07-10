<template>
	<section>
		<div>
			<p>Read existing post</p>
		</div>
	</section>
</template>

<script>
export default {
	validate({ params }) {
		return /^\d+$/.test(params.id)
	}
}
</script>
