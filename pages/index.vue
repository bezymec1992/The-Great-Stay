<template>
	<div class="home-page">
		<Intro>
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<!-- <div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								
							</h1>
							
						</div>
					</div> -->
					<div class="col">
						<div class="background"></div>
						<!-- <picture class="img-holder">
							<source srcset="@/assets/images/img-02.jpg" media="max-widtn: 575px" />
							<img src="@/assets/images/img-01.jpg" alt="Control system for your business" />
						</picture> -->
					</div>
				</div>
			</div>
		</Intro>
		

		<TwoCols>
			<div class="gray-back">
				<div class="woman">
					<div class="container">
						<div class="row">
							<div class="col-md-7">
								<h2 class="h2 two-col-h2 woman-h2">
									Digital support <br/> tool to optimize your revenue
								</h2>
							</div>
							<div class="col-md-5 d-md-flex justify-content-md-end pt-md-5">
								<div class="content-holder">
									<div class="text-holder text-uppercase">
										<p>Our mission</p>
									</div>
									<div class="text-holder text-gray">
										<p>Provide you best tool to manage your place and make your customers excited!</p>
									</div>
								</div>
							</div>
						</div>
						<div class="woman-wrapp">
							<p>
								DISCOVER WHAT CAN WE PROVIDE YOU AND YOUR CUSTOMERS
							</p>
							<picture >
									<source srcset="@/assets/img/woman-mb.jpg" media="(max-width: 600px)" />
									<img src="@/assets/img/woman-desk.jpg" alt="Control system for your business" />
							</picture>
						</div>
					</div>
				</div>
			</div>
		</TwoCols>

		<TwoCols>
			<div class="phones">
				<div class="container">
					<div class="row">
						<div class="col-md-6">
							<p class="phones-span">
								for your hotel
							</p>
							<h2 class="h2 two-col-h2">
								Provide the best experience for your customers
							</h2>
							<p class="phones-span2">
								Organize your workflow and control <br/> every step.
							</p>
							<ul class="d-none d-md-block">
								<li><span>1.</span>  recieve Clients assessment</li>
								<li><span>2.</span> check individual progress of your team</li>
								<li><span>3.</span> manage reports &  complains</li>
							</ul>
						</div>
						<div class="col-md-6 phones-img d-block">
							<picture >
								<source srcset="@/assets/img/02.jpg" media="(max-width: 600px)" width="100%" height="auto"/>
								<img src="@/assets/img/01.jpg" alt="Control system for your business" width="100%" height="auto"/>
							</picture>
							<ul class="d-md-none">
								<li><span>1.</span> recieve Clients assessment</li>
								<li><span>2.</span> check individual progress of your team</li>
								<li><span>3.</span> manage reports &  complains</li>
							</ul>
							<Button type="nuxt-link" to="modules" title="Discover More" class="btn-outline-dark text-capitalize" />
							
						</div>
					</div>
					<div class="img-wrap">
						<picture >
							<source srcset="@/assets/img/04.jpg" media="(max-width: 600px)" width="100%" height="auto"/>
							<img src="@/assets/img/03.jpg" alt="Control system for your business" width="100%" height="auto"/>
						</picture>
					</div>
				</div>
			</div>
		</TwoCols>


		<!-- <div class="brown-holder">
			<SliderPrimary />
			<div class="section-list">
				<div class="container">
					<div class="block">
						<div class="row">
							<div class="col-md-7">
								<div class="content-holder">
									<span class="before-title d-none d-md-block">HAND-HELD MODULE</span>
									<h2 class="h2 d-none d-md-block">Universal mobile application</h2>
									<div class="text-holder txt-m-width-1 d-none d-md-block">
										<p>Your mobile device to take orders from your customers. Internal messages from your colleagues. Be able to send the bill to the app of your customer so you do not even need your terminal.</p>
									</div>
								</div>
							</div>
							<div class="col-md-5">
								<span class="before-title d-md-none">HAND-HELD MODULE</span>
								<h2 class="h2 d-md-none">Universal mobile application</h2>
								<div class="img-holder">
									<img src="@/assets/images/img-05.jpg" alt="phone" />
								</div>
								<div class="text-holder txt-m-width-1 d-md-none">
									<p>Your mobile device to take orders from your customers. Internal messages from your colleagues. Be able to send the bill to the app of your customer so you do not even need your terminal.</p>
								</div>
							</div>
						</div>
					</div>
					<div class="block block-2">
						<div class="row">
							<div class="col-md-7">
								<div class="content-holder">
									<h3 class="h2">A number of opportunities</h3>
									<div class="lists-wrapper">
										<div class="row">
											<div class="col-6">
												<ul class="list">
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-01.svg" alt="icon" />
														</div>
														Payments
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-02.svg" alt="icon" />
														</div>
														Coupons
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-03.svg" alt="icon" />
														</div>
														Shop
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-04.svg" alt="icon" />
														</div>
														Order
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-05.svg" alt="icon" />
														</div>
														Delivery
													</li>
												</ul>
											</div>
											<div class="col-6">
												<ul class="list">
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-06.svg" alt="icon" />
														</div>
														Assistance
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-07.svg" alt="icon" />
														</div>
														Reservation
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-08.svg" alt="icon" />
														</div>
														Chat
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-09.svg" alt="icon" />
														</div>
														Profile
													</li>
													<li>
														<div class="icon-holder">
															<img src="@/assets/images/icon-010.svg" alt="icon" />
														</div>
														Push notifications
													</li>
												</ul>
											</div>
										</div>
									</div>
								</div>
							</div>
							<div class="col-md-5">
								<div class="img-holder">
									<img src="@/assets/images/img-06.jpg" alt="phone" />
								</div>
							</div>
						</div>
					</div>
					<div class="block block-3">
						<div class="row">
							<div class="col-md-7">
								<div class="content-holder">
									<h2 class="h2">Set up notifications to your customers</h2>
									<div class="text-holder txt-m-width-2">
										<p>We help you in your pursuit of customer satisfaction! Always be in touch with your customers.</p>
									</div>
								</div>
							</div>
							<div class="col-md-5">
								<div class="img-holder">
									<img src="@/assets/images/img-07.jpg" alt="phone" />
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div> -->
		<TwoCols class="two-cols-2">
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<div class="col-md-4 d-md-flex align-items-md-start flex-md-column">
						
							<div class="text-holder text-uppercase d-none d-md-block">
								<p>
									Separated flows
								</p>
							</div>
							<ul class="checkboxes-list">
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Receptionist flow
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Cleaning department flow
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Booking & ordering
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Tickets and requests
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Statistics & performance
								</li>
							</ul>
							<Button type="nuxt-link" to="modules" title="I am interested!" class="btn-outline-dark text-capitalize bnt-poss" />
						
					</div>
					<div class="col-md-8">
						<div class="text-holder text-uppercase d-md-none">
							<p>
								Separated flows
							</p>
						</div>
						<h2 class="h2">Just select what you really need</h2>
						<div class="phones-span2">
							We have built separate modules for different department, so you can pick what you need instead overpay for unnecessary functionalities
						</div>
						<div class="img-holder">
							<!-- <img src="@/assets/img/05.png" alt="Pick up Delivery" /> -->
							<picture >
								<source srcset="@/assets/img/06.png" media="(max-width: 600px)" width="100%" height="auto"/>
								<img src="@/assets/img/05.png" alt="Control system for your business" width="100%" height="auto"/>
							</picture>
						</div>
					</div>
					
				</div>
				<div class="slog">
						<h3 class="h3">I think i need a slogan here, in two rows!</h3>
					</div>
			</div>
		</TwoCols>
		<!-- <SliderSecondary /> -->


		<div class="one-col">
			<div class="container">
				<span class="span1">for customer</span>
				<h2 class="h2">At your service <br/> whenever you need us</h2>
				<div class="span2-btn d-flex justify-content-between align-items-center">
					<div class="span2">
						Have full control on departments and response times, so you can be sure that the stay of your clients is amazing.
					</div>
					<div class="btn-wrap d-none d-md-block">
						<Button type="nuxt-link" to="modules" title="Discover More" class="btn-outline-dark text-capitalize btn-one " />
					</div>
				</div>
				<picture >
					<source srcset="@/assets/img/08.png" media="(max-width: 600px)" width="100%" height="auto"/>
					<img src="@/assets/img/07.png" alt="Control system for your business" width="100%" height="auto"/>
				</picture>
				<div class="btn-wrap d-md-none">
					<Button type="nuxt-link" to="modules" title="Discover More" class="btn-outline-dark text-capitalize btn-one " />
				</div>
			</div>
		</div>

		<TwoCols class="two-cols-2 two-cols-2-white">
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<div class="col-md-4 d-md-flex align-items-md-start flex-md-column">
						
							<div class="text-holder text-uppercase d-none d-md-block">
								<p>
									customer’s app
								</p>
							</div>
							<ul class="checkboxes-list">
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									TV channels / Wi-Fi
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Places and people nearby
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Room status
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Services overview
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Dates & prolongation
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Requests & reports
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Bill details
								</li>
							</ul>
							<Button type="nuxt-link" to="modules" title="I am interested!" class="btn-outline-dark text-capitalize bnt-poss" />
						
					</div>
					<div class="col-md-8">
						<div class="text-holder text-uppercase d-md-none">
							<p>
								Separated flows
							</p>
						</div>
						<h2 class="h2">Full control at your finger tips </h2>
						<div class="phones-span2">
							We have collected everything about your stay and hope you will enjoy it! Control your stay, discover places nearby, create special requests. <br/>
							Everything’s possible just with just one app!
						</div>
						<div class="img-holder">
							<!-- <img src="@/assets/img/05.png" alt="Pick up Delivery" /> -->
							<picture >
								<source srcset="@/assets/img/10.png" media="(max-width: 600px)" width="100%" height="auto"/>
								<img src="@/assets/img/09.jpg" alt="Control system for your business" width="100%" height="auto"/>
							</picture>
						</div>
					</div>
					
				</div>
				<div class="slog">
						<h3 class="h3">I think i need a slogan here, in two rows!</h3>
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
// import SliderPrimary from "@/components/Sliders/SliderPrimary";
// import SliderSecondary from "@/components/Sliders/SliderSecondary";
import Contact from "@/components/Sections/Contact";

export default {
	components: {
		Intro,
		Button,
		TwoCols,
		// SliderPrimary,
		// SliderSecondary,
		Contact
	}
};
</script>

<style lang="scss" scoped>
.home-page {
	
	.intro {
		
		min-height: 838px;
		// min-height: calc(var(--vh, 1vh) * 92);

		@include media-breakpoint-up(md) {
			padding-bottom: 26.2rem;
			
		}

		@include media-breakpoint-down(md) {
			min-height: unset;
			// min-height: calc(100vh - 8rem);
			// min-height: calc(var(--vh, 1vh) * 100 - 8rem);
			// padding-bottom: 8rem;
			// background: linear-gradient(90deg, #f4f4f4 0%, #f1f1f1 42.19%, #e8e7e5 100%);

			h1 {
				font-size: 4.8rem;
				margin-bottom: 3rem;
				line-height: 5rem;
			}
		}

		.background {
			@include media-breakpoint-up(md) {
				position: absolute;
				top: 0;
				left: 0;
				width: 100%;
				height: 100%;
				background: url("@/assets/img/main-desk.jpg") no-repeat;
				background-size: cover;
				background-position: center center;
			}

			@include media-breakpoint-down(md) {
				margin-left: -2rem;
				margin-right: -2rem;
				min-height: 73.2rem;
				background: url("@/assets/img/main-mb.jpg") no-repeat;
				background-size: cover;
				background-position: center;
			}

			img {
				width: 100%;
				height: auto;

				@include media-breakpoint-up(md) {
					height: 100%;
					// object-fit: cover;
				}
			}
		}

		// .content-holder {
		// 	@include media-breakpoint-down(md) {
		// 		padding-top: 3.4rem;
		// 	}
		// }
	}
	.gray-back {
		background: #F2F2F2;
	}
	.woman {
		margin-top: 20rem;
		padding-bottom: 10rem;
		background: white;
		border-radius: 0 0 5rem 5rem;
		@include media-breakpoint-down(lg) {
			margin-top: 10rem;
			padding-bottom: 5rem;
			border-radius: 0 0 2rem 2rem;
		}
	}

	.phones {
		background: #F2F2F2;
		padding-top: 20rem;
		@include media-breakpoint-down(lg) {
			padding-top: 8rem;
		}
		.two-col-h2 {
			margin-bottom: 6rem !important;
			@include media-breakpoint-down(lg) {
				margin-bottom: 3.2rem !important;
			}
			
		}
		
		picture {
			max-width: 47rem !important;
		}
		ul {
			padding-left: 0 !important;
			li {
				list-style: none ;
				display: flex;
				border-bottom: 1px solid rgba(7, 7, 7, 0.5);
				@include media-breakpoint-down(lg) {
					font-size: 2rem;
					&:last-child {
						border-bottom: unset;
					}
				}
				padding: 2.5rem 0;
				font-size: 2.4rem;
				text-transform: uppercase;
				span {
					margin-right: 2rem;
					display: block;
					@include media-breakpoint-down(md) {
						margin-right: 1.2rem;
					}
				}
				
				
			}
		}
		
		.phones-img  {
			max-width: 50rem;
			margin-left: auto;
			@include media-breakpoint-down(md) {
				max-width: 100%;
			}
			img {
				border-radius: 20px;
				margin-left: auto;
				margin-bottom: 6rem;
				@include media-breakpoint-down(md) {
					margin-bottom: 4.5rem;
				}
			}
		}
		.img-wrap {
			margin-top: 16rem;
			img {
				border-radius: 25px;
			}
			@include media-breakpoint-down(md) {
				margin-top: 10rem;
			}
		}
	}

	.two-cols {
		.woman-wrapp {
			p {
				margin-bottom: 18rem;
				font-size: 24px;
				line-height: 29px;
				@include media-breakpoint-down(lg) {
					margin-bottom: 4rem;
					font-size: 20px;
					line-height: 30px;
					max-width: 31.5rem;
				}
			}
			
			img {
				width: 100%;
				height: auto;
			}
		}
		.h2 {
			margin-bottom: 8rem;
			font-size: 8rem;
			line-height: 90px;
			@include media-breakpoint-down(md) {
				line-height: 6rem;
				margin-bottom: 4rem;
				font-size: 42px;
				line-height: 50px;
			}
		}
		@include media-breakpoint-down(md) {
			border-radius: 0 0 3rem 3rem;
			// background: red;
		}

		.content-holder {
			max-width: 35rem;
			.text-gray {
				@include media-breakpoint-down(md) {
					font-size: 2rem;
					margin-bottom: 6rem;
				}
			}
		}
	}

	.brown-holder {
		background: #ecdbc7;
		border-bottom-left-radius: 2rem;
		border-bottom-right-radius: 2rem;
		
	}

	.slider-primary {
		background: $white;

		@include media-breakpoint-up(md) {
			border-bottom-left-radius: 2rem;
			border-bottom-right-radius: 2rem;
		}
	}

	.section-list {
		padding-top: 13.7rem;
		padding-bottom: 9.4rem;

		@include media-breakpoint-down(md) {
			padding-top: 8rem;
			padding-bottom: 8rem;
		}

		.block {
			margin-bottom: 5.1rem;

			@include media-breakpoint-down(md) {
				margin-bottom: 8rem;
			}
		}

		.before-title {
			display: block;
			margin-bottom: 2.4rem;
			font-size: 2.4rem;

			@include media-breakpoint-down(md) {
				margin-bottom: 2rem;
				font-size: 1.8rem;
			}
		}

		.text-holder {
			font-size: 2rem;
			line-height: 1.4;
			color: rgba($black, 0.6);

			@include media-breakpoint-down(md) {
				font-size: 1.8rem;
			}

			&.txt-m-width-1 {
				max-width: 60rem;
			}

			&.txt-m-width-2 {
				max-width: 35rem;

				@include media-breakpoint-down(md) {
					margin-bottom: 4rem;
				}
			}
		}

		.content-holder {
			@include media-breakpoint-up(md) {
				margin-right: -0.9rem;
			}
		}

		.img-holder {
			@include media-breakpoint-up(md) {
				padding-left: 0.8rem;
			}

			@include media-breakpoint-down(md) {
				margin-bottom: 4rem;
			}

			img {
				width: 100%;
				height: auto;
				border-radius: 2rem;

				@include media-breakpoint-down(md) {
					border-radius: 1rem;
				}
			}
		}

		.lists-wrapper {
			max-width: 50rem;
		}

		.list {
			margin: 0;
			padding: 0;
			list-style: none;
			font-size: 2.2rem;

			@include media-breakpoint-down(md) {
				margin-bottom: 3.4rem;
				font-size: 1.8rem;
			}

			li {
				display: flex;
				align-items: center;

				&:not(:last-child) {
					margin-bottom: 3rem;

					@include media-breakpoint-down(md) {
						margin-bottom: 1.5rem;
					}
				}
			}

			.icon-holder {
				display: flex;
				margin-right: 2.1rem;

				@include media-breakpoint-down(md) {
					max-width: 2rem;
					margin-right: 1.4rem;
				}

				img {
					width: 100%;
					height: auto;
				}
			}
		}

		.block-2 {
			.h2 {
				@include media-breakpoint-down(md) {
					margin-bottom: 4rem;
				}
			}

			.img-holder {
				@include media-breakpoint-down(md) {
					margin-bottom: 0;
				}
			}
		}

		.block-3 {
			@include media-breakpoint-down(md) {
				margin-bottom: 0;
			}

			.img-holder {
				@include media-breakpoint-down(md) {
					margin-bottom: 0;
				}
			}
		}
	}

	.two-cols-2 {
		padding-top: 18rem;
		margin-bottom: 18rem;
		border-radius: 0 0 30px 30px;
		background: #F2F2F2;
		@include media-breakpoint-down(md) {
			padding-top: 8rem;
			margin-bottom: 8rem;
		}
		.bnt-poss {
			
			@include media-breakpoint-up(md) {
				max-width: 30rem;
			}
		}

		.h2 {
			line-height: 0.9;
			margin-bottom: 5rem !important;
			@include media-breakpoint-down(md) {
				margin-bottom: 3rem !important;
			}
		}

		.checkboxes-list {
			margin-top: auto;
			margin-bottom: 6rem;
			
			@include media-breakpoint-down(md) {
				margin-bottom: 3.6rem;
				li {
					font-size: 20px !important;
				}
			}
		}

		.img-holder {
			@include media-breakpoint-up(xl) {
				width: 80rem;
				height: 52rem;
				margin-top: 4rem;
			}
			@include media-breakpoint-down(md) {
				margin-bottom: 4rem;
			}

			img {
				border-radius: 1rem;
			}
		}
		.slog {
			text-align: center;
			max-width: 738px;
			margin: 18rem auto 0; 
			padding-bottom: 20rem;
			@include media-breakpoint-down(md) {
				margin: 10rem auto 0;
				padding-bottom: 10rem;

			}
			.h3 {
				font-weight: 400;
				font-size: 60px;
				line-height: 80px;
				@include media-breakpoint-down(md) {
					font-size: 32px;
					line-height: 42px;
				}
				
			}
		}
	}

	.one-col {
		margin-bottom: 20rem;
		@include media-breakpoint-down(md) {
			margin-bottom: 10rem;
		}
		.span1 {
			font-size: 24px;
			line-height: 29px;
			text-transform: uppercase;
			@include media-breakpoint-down(md) {
				font-size: 18px;
				line-height: 22px;
			}
		}
		.h2 {
			margin-top: 3rem;
			font-size: 80px;
			line-height: 90px;
			@include media-breakpoint-down(md) {
				font-size: 42px;
				line-height: 50px;
			}
		}
		.span2-btn {
			margin-bottom: 6rem;
			@include media-breakpoint-down(md) {
				margin-bottom: 4rem;
			}
		}
		.span2 {
			font-size: 30px;
			line-height: 40px;
			opacity: 0.6;
			width: 100%;
			max-width: 80rem;
			@include media-breakpoint-down(md) {
				font-size: 20px;
				line-height: 32px;
			}
		}
		.btn-one {
			width: 30rem;
			@include media-breakpoint-down(md) {
				width: 100%;
				margin-top: 5rem;
			}
		}
	}
	.two-cols-2-white {
		background: white;
		padding: 0;
		margin-bottom: 0;
	}
}
</style>
