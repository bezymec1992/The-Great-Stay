<template>
	<div class="app-page">
		<Intro>
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								Hand-Held <br />
								module
							</h1>
							<Button class="btn-outline-dark text-capitalize" type="nuxt-link" to="/contact" title="Request a call" />
						</div>
					</div>
					<div class="col">
						<div class="img-holder">
							<picture>
								<source srcset="@/assets/images/app-intr.jpg" media="(max-width: 768px)" />
								<img src="@/assets/images/img-019.jpg" alt="Control system for your business" />
							</picture>
						</div>
					</div>
				</div>
			</div>
		</Intro>
		<TwoCols>
			<div class="container">
				<div class="row">
					<div class="col-md-6 d-flex flex-md-column justify-content-md-between">
						<h2 class="h2 title">Mobile device to take orders from your customers.</h2>
						<div class="text__wrapper d-none d-md-block">
							<div class="text-holder text-uppercase ">
								<p>Convenient for receiving and placing orders</p>
							</div>
							<div class="text-holder text-gray">
								<p>Internal messages from your colleagues. Be able to send the bill to the app of your customer so you do not even need your terminal.</p>
							</div>
						</div>
					</div>
					<div class="col-md-6">
						<div class="img-holder">
							<picture class="man">
								<source srcset="@/assets/images/img-022.jpg" media="(max-width: 768px)" />
								<img src="@/assets/images/img-021.jpg" alt="Mobile device"/>
							</picture>
						</div>
						<div class="text-holder text-uppercase d-md-none">
							<p>Convenient for receiving and placing orders</p>
						</div>
						<div class="text-holder text-gray d-md-none">
							<p>Internal messages from your colleagues. Be able to send the bill to the app of your customer so you do not even need your terminal.</p>
						</div>
					</div>
				</div>
			</div>
		</TwoCols>
		<div class="shop">
			<div class="container">
				<div class="row">
					<div class="col-12 col-lg-4">
						<h4 class="shop__span">Delivery</h4> 
					</div>
					<div class="col-12 col-lg-8">
						<h2 class="h2 title">Your coffee shop in one app.</h2>
						<div class="row ">
							<div class="shop-wrap col-12 col-xl-6">
								<img class="shop__img" src="../assets/images/img-001.png" alt="pone">
								<h3 class="h3">Menu</h3>
								<p class="shop__text">
									Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consequat tellus pellentesque lorem aliquet. Etiam tempus aliquam at vitae venenatis mauris. 
								</p>
							</div>
							<div class="shop-wrap col-12 col-xl-6">
								<img class="shop__img" src="../assets/images/img-001.png" alt="pone">
								<h3 class="h3">Checkout</h3>
								<p class="shop__text">
									Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consequat tellus pellentesque lorem aliquet. Etiam tempus aliquam at vitae venenatis mauris. 
								</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div class="make">
			<div class="container">
				<div class="make__wrapper d-block">
					<picture class="make-img">
						<source srcset="../assets/images/img-004.jpg" media="(max-width: 768px)" />
						<img src="../assets/images/img-003.jpg" alt="Mobile device to take orders from your customers" />
					</picture>
					<h2 class="h2 make__title">
						Make sure your customers have delicious coffee wherever they are
					</h2>
				</div>
			</div>
		</div>
		<TwoCols>
			<div class="container">
				<div class="row curious">
					<div class="col-12 col-lg-6 d-flex flex-column justify-content-between">
						<h2 class="h2 curious-title">
							Curious about the features of our app?
						</h2>
						<p class="curius-txt">
							Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
						</p>
					</div>
					<div class="col-12 col-lg-6">
						<div class="items">
							<div class="item d-flex">
								<span>1.</span>
								<p class="curius-text">Taking orders</p> 
							</div>
							<div class="item d-flex">
								<span>2.</span>
								<p class="curius-text">Reservation overview</p> 
							</div>
							<div class="item d-flex">
								<span>3.</span>
								<p class="curius-text">Payments</p> 
							</div>
							<div class="item d-flex">
								<span>4.</span>
								<p class="curius-text">Status order</p> 
							</div>
							<div class="item d-flex">
								<span>5.</span>
								<p class="curius-text">Chats</p> 
							</div>
							<div class="item d-flex">
								<span>6.</span>
								<p class="curius-text">Stock Update</p> 
							</div>
						</div>
					</div>
				</div>
			</div>

		</TwoCols>
		<TwoCols>
			<div class="container simple">
				<div class="row simple__wrapper align-items-center">
					<div class="col-12 col-lg-7">
						<h2 class="h2 simple__title">
							It is simple and convenient to use
						</h2>
					</div>
					<div class="col-12 col-lg-5">
						<div class="simple__info d-none d-lg-block">
							<h4>We care about convenience,</h4>
							<p>
								so our app is as intuitive as possible. A few clicks are enough to order, pay or view what you need. 
							</p>
						</div>
					</div>
				</div>
				<div class="simple__picture-wrap">
					<picture class="simple__picture">
						<source srcset="@/assets/images/3-phone-mb.png" media="(max-width: 768px)" />
						<img src="@/assets/images/3-phone-desk.png" alt="Mobile device to take orders from your customers"  />
					</picture>
				</div>
				<div class="simple__info d-lg-none">
					<h4>We care about convenience,</h4>
					<p>
						so our app is as intuitive as possible. A few clicks are enough to order, pay or view what you need. 
					</p>
				</div>
			</div>
		</TwoCols>
		<Contact />
	</div>
</template>

<script>
import Intro from "@/components/Sections/Intro";
import Button from "@/components/Buttons/Button";
import TwoCols from "@/components/Sections/TwoCols";
import Contact from "@/components/Sections/Contact";

export default {
	components: {
		Intro,
		Button,
		TwoCols,
		Contact,
	}
};
</script>

<style lang="scss" scoped>
.app-page {
	.intro {
		position: relative;
		min-height: 90vh;
		min-height: calc(var(--vh, 1vh) * 90);

		@include media-breakpoint-up(md) {
			padding-bottom: 26.2rem;
		}

		@include media-breakpoint-down(md) {
			background: linear-gradient(90deg, #e6e6e4 0%, #e0e0de 9.87%, #e0e0de 20.31%, #dededa 50.97%, #d9d8d4 68.75%, #d4d3cf 85.47%, #d9d8d4 100%);
			min-height: 71.5rem;
			// min-height: calc(var(--vh, 1vh) * 100 - 8rem);
		}

		.img-holder {
			@include media-breakpoint-up(md) {
				position: absolute;
				top: 0;
				left: 0;
				width: 100%;
				height: 100%;
			}

			@include media-breakpoint-down(md) {
				margin-right: -2rem;
				margin-left: -2rem;
				margin-top: -7rem;
				
			}

			img {
				width: 100%;
				height: auto;

				@include media-breakpoint-up(md) {
					height: 100%;
					object-fit: cover;
				}
			}
		}

		// .content-holder {
		// 	@include media-breakpoint-down(md) {
		// 		padding-top: 3.4rem;
		// 	}
		// }
	}
	.title{
		@include media-breakpoint-down(lg) {
			margin-bottom: 4rem;
		}
		
	}
	.man img {
		@include media-breakpoint-up(xl) {
			width: 54rem;
			height: 74rem;
		}
		@include media-breakpoint-down(md) {
			margin-bottom: 4rem;
		}
	}
	.shop {
		padding-top: 20rem;
		padding-bottom: 17.8rem;
		@include media-breakpoint-down(lg) {
			padding-top: 8rem;
			padding-bottom: 8rem;
		}
		.title {
			@include media-breakpoint-down(lg) {
				margin-top: 4rem;
			}
			@include media-breakpoint-down(md) {
				max-width: 33.5rem;
			}
		}
		.shop__img {
			@include media-breakpoint-down(md) {
				width: 100%;
				height: auto;
			}
			margin-bottom: 4rem;
		}
		.shop-wrap {
			@include media-breakpoint-down(md) {
				text-align: left;
			}
			
			margin: 0 auto;
			@include media-breakpoint-down(xl) {
				text-align: center;
				&:first-child {
					margin-bottom: 8rem;
				}
			}

		}
		.shop__text {
			@include media-breakpoint-down(xl) {
				max-width: 33.5rem;
				margin: 0 auto;
			}
			@include media-breakpoint-down(md) {
				margin: 0;
				font-size: 18px;
				line-height: 28px;
				text-align: left;
			}
		}
		.h3 {
			font-size: 5.4rem;
			margin-bottom: 2rem;
			@include media-breakpoint-down(md) {
				font-size: 3rem;
				text-align: left;
			}
		}
		.shop__span {
			text-transform: uppercase;
			font-size: 2.4rem;
			@include media-breakpoint-up(xl) {
				padding-top: 2rem;
				
			}
			@include media-breakpoint-down(lg) {
				font-size: 1.8rem;
			}
		}
	}
	.make {
		.make__wrapper {
			position: relative;
			display: flex;
			justify-content: center;
			align-items: center;
		}
		.make-img img {
			z-index: -1;
			width: 100%;
			height: auto;
		}
		.make__title {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			color: white;
			width: 98.5rem;
			max-width: 100%;
			@include media-breakpoint-down(md) {
				left: 45%;
			}
			@include media-breakpoint-down(lg) {
				font-size: 3rem;
				width: 28rem;
				max-width: 100%;
			}
		}
	}
	.curious {
		display: flex;
		justify-content: space-between;
		.curius-txt {
			max-width: 35.8rem;
			font-size: 20px;
			opacity: 0.6;
			
			@include media-breakpoint-down(lg) {
				margin: 0 auto 4rem;
				text-align: center;
			}
			@include media-breakpoint-down(md) {
				margin: 0 0 4rem;
				text-align: left;
			}
		}
		.curious-title {
			@include media-breakpoint-down(lg) {
				text-align: center;
			}
			@include media-breakpoint-down(md) {
				text-align: left;
			}
		}
		.items {
			margin-left: auto;
		}
		.item {
			margin-left: auto;
			border-bottom: 1px solid gray;
			max-width: 47rem;
			padding-bottom: 2.5rem;
			font-size: 2.4rem;
			@include media-breakpoint-down(lg) {
				margin: 0 auto;
				font-size: 2rem;
			}
			&:not(:last-child) {
				margin-bottom: 2.5rem;
			}
			p {
				margin-left: 5rem;
				text-transform: uppercase;
				margin-bottom: 0;
				
			}
		}
	}
	.simple {
		padding-bottom: 200px;
		@include media-breakpoint-down(lg) {
			padding-bottom: 80px;
		}
		.simple__wrapper {
			@include media-breakpoint-up(lg) {
				margin-bottom: 194px;
			}
		}
		.simple__title {
			line-height: 94px;
			margin-bottom: 0;
			@include media-breakpoint-down(lg) {
				line-height: 60px;
				margin-bottom: 40px;
			}
		}
		.simple__picture img {
			width: 100%;
			height: auto;
		}
		.simple__picture-wrap {
			@include media-breakpoint-down(md) {
				margin-left: -2rem;
				margin-right: -2rem;
			}
			@include media-breakpoint-down(lg) {
				margin-bottom: 40px;
			}
		}
		.simple__info {
			max-width: 35rem;
			@include media-breakpoint-up(lg) {
				margin-left: auto;
			}
			h4 {
				font-size: 20px;
				text-transform: uppercase;
				margin-bottom: 30px;
				@include media-breakpoint-down(lg) {
					margin-bottom: 20px;
				}
			}
			p {
				font-size: 20px;
				opacity: 0.6;
				@include media-breakpoint-down(lg) {
					font-size: 18px;
				}
			}
		}
	}
}
</style>
