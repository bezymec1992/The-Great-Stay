<template>
	<div class="intro">
		<slot />
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.intro {
	position: relative;
	// padding-top: 21.6rem;
	padding-bottom: 8rem;
	@include media-breakpoint-down(md) {
		padding-top: 0;
		padding-bottom: 0rem;
	}

	.content-holder {
		position: relative;
		z-index: 2;
	}
}
</style>
