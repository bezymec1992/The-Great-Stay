<template>
	<transition v-if="isOpen" name="fade">
		<div class="modal-overlay" @click="handleClose">
			<div class="modal" @click.stop>
				<a href="#" class="close-icon" @click.prevent="handleClose">
					<svg width="29" height="30" viewBox="0 0 29 30" fill="none" xmlns="http://www.w3.org/2000/svg">
						<line x1="0.353553" y1="0.646447" x2="28.6378" y2="28.9307" stroke="black" />
						<line x1="28.6377" y1="1.35355" x2="0.353462" y2="29.6378" stroke="black" />
					</svg>
				</a>
				<slot name="modal-body" />
			</div>
		</div>
	</transition>
</template>

<script>
export default {
	name: "Modal",
	data() {
		return {
			isOpen: false
		};
	},
	methods: {
		handleOpen() {
			this.isOpen = true;

			const scrollWidth = window.innerWidth - document.getElementsByTagName("html")[0].clientWidth;
			document.body.style.paddingRight = scrollWidth + "px";
			document.body.style.overflow = "hidden";
		},
		handleClose() {
			this.isOpen = false;

			setTimeout(() => {
				document.body.style.removeProperty("padding-right");
				document.body.style.removeProperty("overflow");
			}, 250);
		}
	}
};
</script>

<style lang="scss" scoped>
.modal-overlay {
	position: fixed;
	top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	background-color: #000000da;
	z-index: 100;
	display: flex;
	align-items: center;
	justify-content: center;
	z-index: 101;

	.modal {
		position: relative;
		width: 100%;
		max-width: 94rem;
		background-color: $white;
		overflow: auto;

		@include media-breakpoint-down(lg) {
			max-width: 100%;
			height: 100%;
		}
	}

	.close-icon {
		position: absolute;
		top: 4rem;
		right: 4rem;
		display: inline-block;
		width: 2.3rem;

		@include media-breakpoint-down(lg) {
			top: 3rem;
			right: 3.5rem;
			width: 2rem;
		}

		svg {
			width: 100%;
			height: 100%;
		}
	}

	&.contact-from {
		.modal {
			@include media-breakpoint-up(lg) {
				max-width: 60rem;
			}

			@include media-breakpoint-down(md) {
				padding-left: 2rem;
				padding-right: 2rem;
				border-radius: 0;
			}
		}
	}

	.modal-request {
		padding: 7rem 4rem;
	}
}
</style>
