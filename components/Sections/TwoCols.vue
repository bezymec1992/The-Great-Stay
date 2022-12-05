<template>
	<div class="two-cols">
		<slot />
	</div>
</template>

<style lang="scss" scoped>
.two-cols {
	// padding-top: 17.8rem;

	// @include media-breakpoint-down(md) {
	// 	padding-top: 8rem;
	// }
	// border-radius: 0 0 5rem 5rem;
	// background: #f68888;
	
	@include media-breakpoint-down(md) {
		// border-radius: 0 0 2rem 2rem;
	}

	.img-holder {
		img {
			width: 100%;
			height: auto;
		}
	}

	.h2 {
		line-height: 0.9;
	}

	.text-holder {
		margin-bottom: 3rem;

		@include media-breakpoint-down(md) {
			margin-bottom: 2rem;
			font-size: 1.8rem;
			line-height: 1.5;
		}

		&.text-gray {
			color: rgba($black, 0.6);
		}
	}

	.phones-span {
			font-size: 24px;
			margin-bottom: 3.5rem;
			text-transform: uppercase;
			@include media-breakpoint-down(lg) {
				font-size: 18px;
				margin-bottom: 2rem;
			}
		}
		.phones-span2 {
			font-size: 30px;
			line-height: 40px;
			opacity: 0.6;
			@include media-breakpoint-down(lg) {
				font-size: 20px;
				line-height: 32px;
				margin-bottom: 4rem;
			}
		}
}
</style>
