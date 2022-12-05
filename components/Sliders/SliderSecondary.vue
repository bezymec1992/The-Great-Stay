<template>
	<div class="slider-secondary">
		<div class="container">
			<TwoCols class="pt-0">
				<div class="row">
					<div class="col-md-7">
						<h2 class="h2 d-none d-md-block">
							Liked our system? <br />
							We can customize it for you!
						</h2>
						<div class="text-holder text-uppercase d-none d-md-block">
							<p>We also can work together if you have...</p>
						</div>
					</div>
					<div class="col-md-5 d-flex flex-md-column flex-column-reverse align-items-md-end">
						<div class="content-holder">
							<div class="text-holder text-uppercase">
								<p>We are open to cooperation with various businesses!</p>
							</div>
							<div class="text-holder text-gray text-holder2">
								<p>We are very flexible and ready to cooperate and adapt to different types of business.</p>
							</div>
						</div>
						<ul class="swiper-nav">
							<li>
								<button class="btn-swiper slider-secondary-btn-prev btn-prev">
									<div class="icon-holder">
										<img src="@/assets/images/icon-arrow-right.svg" alt="icon arrpw prev" />
									</div>
								</button>
							</li>
							<li>
								<button class="btn-swiper slider-secondary-btn-next btn-next">
									<div class="icon-holder">
										<img src="@/assets/images/icon-arrow-right.svg" alt="icon arrpw prev" />
									</div>
								</button>
							</li>
						</ul>
					</div>
				</div>
			</TwoCols>
			<div class="safe-holder">
				<div class="swiper-titles">
					<h2 class="h2 d-md-none">Liked our system? We can customize it for you!</h2>
					<div class="text-holder text-uppercase d-md-none">
						<p>We also can work together if you have...</p>
					</div>
				</div>

				<swiper class="swiper" :options="swiperOption" ref="swiper">
					<swiper-slide>
						<div class="slide-inner">
							<h3 class="h3">COFFEE SHOP</h3>
							<div class="img-holder">
								<picture>
									<source srcset="@/assets/images/img-09.jpg" media="max-widtn: 575px" />
									<img src="@/assets/images/img-09.1.jpg" alt="img alt" />
								</picture>
							</div>
						</div>
					</swiper-slide>
					<swiper-slide>
						<div class="slide-inner">
							<h3 class="h3">RESTAURANT</h3>
							<div class="img-holder">
								<picture>
									<source srcset="@/assets/images/img-09.jpg" media="max-widtn: 575px" />
									<img src="@/assets/images/img-09.jpg" alt="img alt" />
								</picture>
							</div>
						</div>
					</swiper-slide>
					<swiper-slide>
						<div class="slide-inner">
							<h3 class="h3">CAFE</h3>
							<div class="img-holder">
								<picture>
									<source srcset="@/assets/images/img-09.jpg" media="max-widtn: 575px" />
									<img src="@/assets/images/img-09.3.jpg" alt="img alt" />
								</picture>
							</div>
						</div>
					</swiper-slide>
				</swiper>
			</div>
		</div>
	</div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import TwoCols from "@/components/Sections/TwoCols";
import "swiper/css/swiper.css";

export default {
	name: "SliderPrimary",
	components: {
		Swiper,
		SwiperSlide,
		TwoCols
	},

	data() {
		return {
			swiperOption: {
				slidesPerView: 1.1,
				// direction: "vertical",
				speed: 1100,
				// mousewheel: {
				// 	releaseOnEdges: true
				// },
				spaceBetween: 10,
				// autoplay: {
				// 	delay: 5000
				// },
				navigation: {
					nextEl: ".slider-secondary-btn-next",
					prevEl: ".slider-secondary-btn-prev"
				},
				breakpoints: {
					768: {
						slidesPerView: 2.2,
						spaceBetween: 40
					}
				}
			}
		};
	}
};
</script>

<style lang="scss" scoped>
.slider-secondary {
	padding-bottom: 12.6rem;
	overflow: hidden;
	.h2 {
		line-height: 9.4rem;
		margin-bottom: 10rem;
		@include media-breakpoint-down(lg) {
			line-height: 6rem;
			margin-bottom: 4rem;
		}
	}
	@include media-breakpoint-down(md) {
		padding-bottom: 7rem;
	}

	> .container {
		@include media-breakpoint-down(md) {
			display: flex;
			flex-direction: column-reverse;
		}
	}

	.text-holder {
		margin-bottom: 6.2rem;
		font-size: 2.4rem;
		line-height: 1.16;

		@include media-breakpoint-down(md) {
			margin-bottom: 2rem;
			font-size: 1.8rem;
		}
	}

	.text-holder2 {
		font-size: 20px;
		@include media-breakpoint-up(md) {
			margin-bottom: 4.7rem;
		}
	}

	.slide-inner {
		position: relative;
		display: flex;
		align-items: center;
		justify-content: center;
		color: $white;
		min-height: 52rem;

		@include media-breakpoint-down(md) {
			min-height: 32rem;
		}

		.h3 {
			position: relative;
			font-size: 2.4rem;
			z-index: 3;
		}

		&::before {
			content: "";
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			background: rgba($black, 0.2);
			z-index: 1;
			border-radius: 1rem;
		}

		.img-holder {
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;

			img {
				width: 100%;
				height: 100%;
				object-fit: cover;
				border-radius: 1rem;
			}
		}
	}

	.swiper-nav {
		@include media-breakpoint-up(md) {
			padding-top: 0;
		}

		@include media-breakpoint-down(md) {
			padding-bottom: 4rem;
		}
	}

	.swiper-titles {
		@include media-breakpoint-down(md) {
			padding-bottom: 1rem;
		}
	}

	.two-cols {
		.content-holder {
			max-width: 38rem;
			
			@include media-breakpoint-up(md) {
				padding-top: 2rem;
				margin-bottom: 13rem;

			}
		}
	}
}
</style>

<style lang="scss">
.slider-secondary {
	.swiper {
		overflow: visible;
	}
}
</style>
