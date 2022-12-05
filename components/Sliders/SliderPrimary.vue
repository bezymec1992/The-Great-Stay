<template>
	<div class="slider-primary">
		<div class="container">
			<div class="text-holder text-uppercase">
				<p>POS & CRM MODULE AND CMS MODULE</p>
			</div>
			<swiper class="swiper" :options="swiperOption" ref="swiper">
				<swiper-slide>
					<div class="slide-inner">
						<div class="img-holder">
							<picture>
								<source srcset="@/assets/images/img-04.png" media="max-widtn: 575px" />
								<img src="@/assets/images/img-03.png" alt="img alt" />
							</picture>
						</div>
					</div>
				</swiper-slide>
				<swiper-slide>
					<div class="slide-inner">
						<div class="img-holder">
							<picture>
								<source srcset="@/assets/images/img-04.png" media="max-widtn: 575px" />
								<img src="@/assets/images/img-03.png" alt="img alt" />
							</picture>
						</div>
					</div>
				</swiper-slide>
				<swiper-slide>
					<div class="slide-inner">
						<div class="img-holder">
							<picture>
								<source srcset="@/assets/images/img-04.png" media="max-widtn: 575px" />
								<img src="@/assets/images/img-03.png" alt="img alt" />
							</picture>
						</div>
					</div>
				</swiper-slide>
			</swiper>
			<ul class="swiper-nav">
				<li>
					<button class="btn-swiper slider-primary-btn-prev btn-prev">
						<div class="icon-holder">
							<img src="@/assets/images/icon-arrow-right.svg" alt="icon arrpw prev" />
						</div>
					</button>
				</li>
				<li>
					<button class="btn-swiper slider-primary-btn-next btn-next">
						<div class="icon-holder">
							<img src="@/assets/images/icon-arrow-right.svg" alt="icon arrpw prev" />
						</div>
					</button>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
	name: "SliderPrimary",
	components: {
		Swiper,
		SwiperSlide
	},

	data() {
		return {
			swiperOption: {
				slidesPerView: 1,
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
					nextEl: ".slider-primary-btn-next",
					prevEl: ".slider-primary-btn-prev"
				},
				breakpoints: {
					768: {
						// freeMode: true
						spaceBetween: 40
					}
				}
			}
		};
	}
	// methods: {
	// 	prev() {
	// 		this.$refs.swiper.$swiper.slidePrev();
	// 	},
	// 	next() {
	// 		this.$refs.swiper.$swiper.slideNext();
	// 	}
	// }
};
</script>

<style lang="scss" scoped>
.slider-primary {
	padding-bottom: 12.6rem;
	overflow: hidden;

	@include media-breakpoint-down(md) {
		padding-bottom: 8rem;
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

	.slide-inner {
		display: flex;
		align-items: center;
		justify-content: center;
		padding-top: 7rem;
		padding-bottom: 3rem;
		background: #f5f5f5;
		border: 0.1rem solid #000000;
		border-radius: 2rem;

		@include media-breakpoint-down(md) {
			padding: 6.6rem 0.7rem;
		}

		.img-holder {
			max-width: 79.5rem;

			img {
				width: 100%;
				height: auto;
			}
		}
	}
}
</style>

<style lang="scss">
.slider-primary {
	.swiper {
		overflow: visible;
	}
}
</style>
