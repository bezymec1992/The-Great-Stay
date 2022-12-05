<template>
	<div class="app-page">
		<Intro>
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								Choose the best modules for your business
							</h1>
							<Button class="btn-outline-dark text-capitalize" type="nuxt-link" to="/contact" title="Request a call" />
						</div>
					</div>
					<div class="col">
						<div class="img-holder">
							<picture>
								<source srcset="@/assets/images/mmb.jpg" media="(max-width: 768px)" />
								<img src="@/assets/images/module-main-desk.jpg" alt="Control system for your business" />
							</picture>
						</div>
					</div>
				</div>
			</div>
		</Intro>

		<div class="icons">
			<div class="container">
				<div class="icons__wrapper row d-flex justify-content-between">
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-001.svg" alt="icon">
						<h4>Reservation <br/> module</h4>
					</div>
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-002.svg" alt="icon">
						<h4>Pick up <br/> & delivery</h4>
					</div>
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-003.svg" alt="icon">
						<h4>Loyalty <br/> & gamification</h4>
					</div>
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-004.svg" alt="icon">
						<h4>Shop <br/> module</h4>
					</div>
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-005.svg" alt="icon">
						<h4>Terrace <br/> module</h4>
					</div>
					<div class="icons-icon col-4 col-lg-2 d-flex flex-column align-items-center text-center">
						<img src="@/assets/images/icon-006.svg" alt="icon">
						<h4>Modular <br/> CRM</h4>
					</div>
				</div>
			</div>
		</div>
		
		<div class="girl girl-1">
			<div class="container">
				<div class="row">
					<div class="col-12 col-lg-4">
						<h4 class="h4 ">Loyalty & gamification</h4>
					</div>
					<div class="col-12 col-lg-8">
						<h2 class="h2 mb-5">Reward your clients for their visit.</h2>
					</div>
				</div>
				<div class="row">
					<div class="col-12 col-lg-4 done-wrap mt-auto mb-5 mb-lg-0">
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Engage with your clients</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Compete & Reward</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Make it fun</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Make them come back and share their loyalty with others</p>
						</div>
					</div>
					<div class="col-12 col-lg-8">
						<picture class="girl-picture">
							<source srcset="@/assets/images/img-006.jpg" media="(max-width: 768px)" width="100%" height="auto" />
							<img src="@/assets/images/img-005.jpg" alt="girl" width="100%" height="auto"/>
						</picture>
					</div>
				</div>
				<p class="girl-text">
					Reward your clients for their visit. Having all their benefits on their phone. Be in the pocket of your customer.
				</p>
			</div>
		</div>

		<div class="girl girl-2">
			<div class="container">
				<div class="row">
					<div class="col-12 col-lg-7">
						<h4 class="h4 h4-girl">TERRACE MODULE</h4>
						<h2 class="h2 mb-5">Take care of your customers' time and convenience </h2>
						<p class="girl-text girl-text2">
							It is busy people are waiting…They want to pay …. One of your employees called sick during a sunny day…. They forgot to bring the spoon for the soup. Customers are getting more and more used to possibility on ordering themselves if it benefits them. 
						</p>
					</div>
					<div class="col-12 col-lg-5 done-2 ml-auto d-none d-lg-block">
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Order</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Pay yourself</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Assistance</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Inspiring menu, even with video</p>
						</div>
					</div>
				</div>
				<picture>
					<source srcset="@/assets/images/img-008.jpg" media="(max-width: 768px)" width="100%" height="auto" />
					<img src="@/assets/images/img-007.jpg" alt="girl" width="100%" height="auto"/>
				</picture>

				<div class="col-12 col-lg-5 done-2 ml-0 d-lg-none">
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Order</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Pay yourself</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Assistance</p>
						</div>
						<div class="done d-flex">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Inspiring menu, even with video</p>
						</div>
					</div>
			</div>
		</div>

		<div class="reserve">
			<div class="container">
				<div class="row">
					<div class="col-12 col-lg-4">
						<p class="reserve-mod">RESERVATION MODULE</p>
					</div>
					<div class="col-12 col-lg-8">
						<h2 class="h2 reserve-title">Simple table reservation system</h2>
						<div class="reserve-done d-flex">
							<div class="done d-flex align-items-center">
								<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
								<p class="done-text">Good overview </p>
							</div>
							<div class="done d-flex align-items-center">
								<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
								<p class="done-text">Block tables </p>
							</div>
							<div class="done d-flex align-items-center">
								<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
								<p class="done-text">Give preference to loyal customers </p>
							</div>
						</div>
						<picture class="reserve-picture">
							<source srcset="@/assets/images/img-0010.jpg" media="(max-width: 768px)" width="100%" height="auto" />
							<img src="@/assets/images/img-009.jpg" alt="girl" width="100%" height="auto"/>
						</picture>
						<p class="reserve-text">
							Easy flow to make a reservation for your customers. You decide when and which tables to make available.
						</p>
					</div>
				</div>
			</div>
		</div>

		<div class="girl girl-1">
			<div class="container">
				<div class="row">
					<div class="col-12 col-lg-4">
						<h4 class="h4 mt-md-4">SHOP MODULE</h4>
					</div>
					<div class="col-12 col-lg-8">
						<h2 class="h2 mb-5">Store in the client's pocket</h2>
					</div>
				</div>
				<div class="row">
					<div class="col-12 col-lg-4 done-wrap mt-auto mb-5 mb-lg-0">
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Gift cards</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Own coffee beans</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Other products</p>
						</div>
						<div class="done d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done-icon" width="24" height="24">
							<p class="done-text">Merchandising</p>
						</div>
					</div>
					<div class="col-12 col-md-6 col-lg-4 mb-5 mb-md-0">
						<picture>
							<source srcset="@/assets/images/img-006.jpg" media="(max-width: 168px)" width="100%" height="auto" />
							<img src="@/assets/images/img-002.png" alt="girl" width="100%" height="auto"/>
						</picture>
					</div>
					<div class="col-12 col-md-6 col-lg-4">
						<picture>
							<source srcset="@/assets/images/img-006.jpg" media="(max-width: 168px)" width="100%" height="auto" />
							<img src="@/assets/images/img-001.png" alt="girl" width="100%" height="auto"/>
						</picture>
					</div>
				</div>
				<p class="girl-text">
					24/7 open. The opportunity to upsell. Give your clients the opportunity to buy products even when you are closed.
				</p>
			</div>
		</div>

		<div class="cup">
			<div class="container">
				<div class="cup__wrapp">
					<h4>PICK UP & DELIVERY</h4>
					<h2 class="h2">
						Give your customers the opportunity to order to enjoy products anywhere.
					</h2>
					<div class="cup__items d-none d-md-flex">
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Pick up in store </p>
						</div>
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Pre order and pay </p>
						</div>
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Deliver to my office or house</p>
						</div>
					</div>
					<picture>
						<source srcset="@/assets/images/img-0012.jpg" media="(max-width: 768px)" width="100%" height="auto" />
						<img src="@/assets/images/img-0011.jpg" alt="girl" width="100%" height="auto"/>
					</picture>
					<div class="cup__items d-block d-md-none">
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Pick up in store </p>
						</div>
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Pre order and pay </p>
						</div>
						<div class="cup__item d-flex align-items-center">
							<img src="@/assets/images/img-done.png" alt="done icon">
							<p class="mb-0">Deliver to my office or house</p>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<Contact />
	</div>
</template>

<script>
import Intro from "@/components/Sections/Intro";
import Button from "@/components/Buttons/Button";
import Contact from "@/components/Sections/Contact";
export default {
	components: {
		Intro,
		Button,
		Contact,
	}
};
</script>

<style lang="scss" scoped>
	
.app-page {
	.intro {
		display: flex;
		align-items: end;
		position: relative;
		
		min-height: 90vh;
		min-height: calc(var(--vh, 1vh) * 90);
		margin-bottom: 19rem;
		@include media-breakpoint-up(md) {
			padding-bottom: 26.2rem;
		}
		

		@include media-breakpoint-down(md) {
			// background: linear-gradient(90deg, #e6e6e4 0%, #e0e0de 9.87%, #e0e0de 20.31%, #dededa 50.97%, #d9d8d4 68.75%, #d4d3cf 85.47%, #d9d8d4 100%);
			background: url("@/assets/images/module-intr.jpg");
			background-size: cover;
			background-repeat: no-repeat;
			background-position: center;
			min-height: 75.5rem;
			margin-bottom: 8rem;
			
			top: -5rem;

			h1 {
				margin-bottom: 3rem;
			}
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
				display: none;
				margin-right: -2rem;
				margin-left: -2rem;
				margin-bottom: 0;
				
				
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

		.content-holder {
			@include media-breakpoint-down(md) {
				padding-top: 0;
				position: relative;
				top: -7rem;
				h1 {
					font-size: 4rem;
					margin-bottom: 2rem;
				}
				
			}
		}
	}
	.title, .img-holder {
		@include media-breakpoint-down(lg) {
			margin-bottom: 4rem;
		}
		
	}
	.icons {
		padding-bottom: 20rem;
		@include media-breakpoint-down(md) {
			padding-bottom: 4rem;
		}
		.icons-icon {
			padding-left: 0;
			padding-right: 0;
			@include media-breakpoint-down(lg) {
				margin-bottom: 4rem;
			}
			img {
				margin-bottom: 3.6rem;
				@include media-breakpoint-down(lg) {
					width: 2.1rem;
					height: 2.1rem;
					margin-bottom: 1.6rem;
				}
			}
			
			h4 {
				@include media-breakpoint-down(lg) {
					font-size: 1.4rem;
				}
				font-size: 2rem;
				text-transform: uppercase;
			}
		}
		

	}
	
	.girl {
		.girl-picture img{
			@include media-breakpoint-up(xl) {
				width: 80rem;
				height: 52rem;
			}
		}
		h4 {
			font-size: 2.4rem;
			text-transform: uppercase;
			padding-top: 10px;

			@include media-breakpoint-down(lg) {
				padding-bottom: 4rem;
				margin-bottom: 0;
				font-size: 1.8rem;
				padding-top: 0;
			}
		}
		.girl-text {
			max-width: 79rem;
			@include media-breakpoint-up(xl) {
				max-width: 80rem;
				margin-right: -2rem;
			}
			margin-left: auto;
			opacity: 0.6;
			margin-top: 6rem;
			@include media-breakpoint-down(lg) {
				margin-left: 0;
				margin-top: 4rem;
				font-size: 1.8rem;
			}
		}
		.done-text {
			font-size: 2.2rem;
			opacity: 0.6;
			padding-left: 2rem;
			max-width: 33.6rem;
			margin-bottom: 0;
		}
		.done:not(:last-child) {
			margin-bottom: 2.5rem;
			@include media-breakpoint-down(lg) {
				margin-bottom: 2rem;
			}
		}
		
	}

	.girl-1, .girl-2 {
		padding-bottom: 19rem;
		@include media-breakpoint-down(lg) {
			padding-bottom: 8rem;
		}
		
		.girl-text2 {
			margin-bottom: 8rem;
			margin-top: 0;
			padding-top: 0;
			max-width: 61.7rem;
			margin-left: 0;
			@include media-breakpoint-down(lg) {
				margin-bottom: 4rem;
			}
		}

		.h4-girl {
			margin-bottom: 4rem;
			@include media-breakpoint-down(lg) {
				margin-bottom: 0;
			}
		}

		.done-2 {
			margin-top: 12rem;
			margin-left: auto;
			max-width: 400px;

			@include media-breakpoint-down(lg) {
				margin-left: 0;
				margin-top: 4rem;
			}
		}
	}

	.reserve {
		padding-bottom: 20rem;
		.reserve-mod {
			margin-top: 2rem;
			margin-bottom: 0;

			@include media-breakpoint-down(lg) {
				margin-top: 0;
			}
		}
		@include media-breakpoint-down(lg) {
			padding-bottom: 8rem;
			.reserve-mod, .reserve-title {
				margin-bottom: 4rem;
			}
		}
		
		.done-text {
			margin-bottom: 0;
			margin-left: 1.5rem;
			opacity: 0.6;
		}
		.reserve-done {
			margin-bottom: 6rem;
			justify-content: space-between;

			@include media-breakpoint-down(xl) {
				flex-direction: column;
				margin-bottom: 4rem;
				.done:not(:last-child) {
					margin-bottom: 2rem;
				}
			}
		}
		.reserve-text{
			margin-top: 4rem;
			opacity: 0.6;
		}
	}
	
	.cup {
		padding-bottom: 20rem;

		@include media-breakpoint-down(lg) {
			padding-bottom: 8rem;
		}
		.cup__wrapp {
			h2 {
				max-width: 103rem;
				margin-bottom: 6rem;

				@include media-breakpoint-down(md) {
					margin-bottom: 4rem;
				}
			}
			h4 {
				font-size: 2rem;
				text-transform: uppercase;
				margin-bottom: 4rem;

				@include media-breakpoint-down(md) {
					font-size: 1.8rem;
				}
			}
			
		}
		.cup__items {
			max-width: 80rem;
			justify-content: space-between;
			margin-bottom: 6rem;

			@include media-breakpoint-down(md) {
				margin-top: 4rem;
				margin-bottom: 0;
			}
		}
		.cup__item {
			@include media-breakpoint-down(md) {
				&:not(:last-child) {
					margin-bottom: 2rem;
				}
			}
		}
		.cup__item p{
			padding-left: 2rem;
			opacity: 0.6;
			font-size: 2.2rem;

			@include media-breakpoint-down(lg) {
				font-size: 1.8rem;
			}
		}
	}
	
}
</style>
