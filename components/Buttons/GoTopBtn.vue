<template>
	<transition name="fade">
		<button v-if="isShow" class="go-to-top" @click="scrollToTop()">
			<span class="arrow-holder"
				><svg width="24" height="26" viewBox="0 0 24 26" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M13.0607 0.939341C12.4749 0.353554 11.5251 0.353554 10.9393 0.939341L1.3934 10.4853C0.807611 11.0711 0.807611 12.0208 1.3934 12.6066C1.97918 13.1924 2.92893 13.1924 3.51472 12.6066L12 4.12132L20.4853 12.6066C21.0711 13.1924 22.0208 13.1924 22.6066 12.6066C23.1924 12.0208 23.1924 11.0711 22.6066 10.4853L13.0607 0.939341ZM13.5 25.25L13.5 2L10.5 2L10.5 25.25L13.5 25.25Z" fill="white" />
				</svg>
			</span>
		</button>
	</transition>
</template>

<script>
import smoothscroll from "smoothscroll-polyfill";

export default {
	name: "GoTopBtn",
	data: () => ({
		isShow: false
	}),
	mounted() {
		window.addEventListener("scroll", this.handleScroll);
		smoothscroll.polyfill();
	},
	methods: {
		scrollToTop() {
			window.scrollTo({
				top: 0,
				behavior: "smooth"
			});
		},
		handleScroll() {
			if (pageYOffset >= 500) {
				this.isShow = true;
			} else {
				this.isShow = false;
			}
		}
	}
};
</script>

<style lang="scss" scoped>
.go-to-top {
	position: fixed;
	right: 3rem;
	bottom: 6rem;
	width: 7.2rem;
	height: 7.2rem;
	display: flex;
	align-items: center;
	justify-content: center;
	background: rgba($black, 0.3);
	border: none;
	border-radius: 50%;
	transition: $transition;
	z-index: 10;

	@include media-breakpoint-down(md) {
		right: 1.5rem;
		bottom: 6rem;
		width: 5rem;
		height: 5rem;
	}

	&:hover {
		background: rgba($black, 1);
	}

	.arrow-holder {
		display: flex;

		@include media-breakpoint-down(md) {
			width: 1.7rem;
		}

		img {
			width: 100%;
			height: auto;
		}
	}
}

.fade-enter-active,
.fade-leave-active {
	transition: opacity 0.5s;
}
.fade-enter,
.fade-leave-to {
	opacity: 0;
}
</style>
