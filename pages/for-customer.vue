<template>
    <div class="wr">
        <Intro>
			<div class="container">
				<div class="intr-wrapp">
                
                    <h1>At your service whenever you need us</h1>
					<a href="#col">
						<img src="@/assets/img/sc.svg" alt="">
					</a>
					<!-- <div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								
							</h1>
							
						</div>
					</div> -->
					<div class="intr-img">
						<div class="intr-img-wrap">
							<picture>
								<source srcset="@/assets/img/custom-m.png" media="(max-width: 1200px)" />
								<img src="@/assets/img/custom-d.png" alt="Control system for your business" width="100%" height="auto"/>
							</picture>
						</div>
					</div>
				</div>
			</div>
		</Intro>
        <TwoCols class="two-cols-2 two-cols-2-white">
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<div class="col-md-4 d-md-flex align-items-md-start flex-md-column justify-content-between">
						
							<div class="text-holder text-uppercase d-none d-md-block">
								<p>
									Your great stay
								</p>
							</div>
							<ul class="checkboxes-list">
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									User friendly
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Consists important info
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Full of additional options
								</li>
								<li>
									<div class="icon-holder">
										<img src="@/assets/img/done.svg" alt="icon of checkbox" />
									</div>
									Quick response
								</li>
								
							</ul>
					</div>
					<div class="col-md-8">
						<div class="text-holder text-uppercase d-md-none">
							<p>
								your great stay
							</p>
						</div>
						<h2 class="h2">Full control at <br class="d-md-none"/> your finger<br class="d-md-none"/> tips </h2>
						<div class="phones-span2 d-md-none">
							All the services I need in my pocket. Easy access to all the services during your stay.
						</div>
						<div class="img-holder">
							<picture >
								<source srcset="@/assets/img/10.png" media="(max-width: 600px)" width="100%" height="auto"/>
								<img src="@/assets/img/09.jpg" alt="Control system for your business" width="100%" height="auto"/>
							</picture>
						</div>
                        <div class="phones-span2 d-none d-md-block">
							All the services I need in my pocket. Easy access to all the services during your stay.
						</div>
					</div>
				</div>
			</div>
		</TwoCols>
        <div class="quick">
            <div class="container">
                <h2 class="h2">Quick app overview</h2>
                <div class="quick-wrap">
                    <div class="quick__item">
                        <img src="@/assets/img/q1.svg" alt="">
                        <p>TV channels</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q2.svg" alt="">
                        <p>Wi-Fi password</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q3.svg" alt="">
                        <p>Places nearby</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q4.svg" alt="">
                        <p>Room status</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q5.svg" alt="">
                        <p>Services overview</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q6.svg" alt="">
                        <p>Bill details</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q7.svg" alt="">
                        <p>Dates & prolongation</p>
                    </div>
                    <div class="quick__item">
                        <img src="@/assets/img/q8.svg" alt="">
                        <p>Requests & reports</p>
                    </div>
                </div>
            </div>
        </div>

        <TwoCols>
			<div class="phones">
				<div class="container">
					<div class="row">
						<div class="col-md-6">
							
							<h2 class="h2 two-col-h2">
								Create special requests
							</h2>
							<p class="phones-span2">
								Want something we don’t have? Make a request and we will try to help you.
							</p>
							<ul class="d-none d-md-block">
								<li><span>1.</span>Meeting rooms</li>
								<li><span>2.</span>ironing / laudry</li>
								<li><span>3.</span>Special orders</li>
							</ul>
						</div>
						<div class="col-md-6 phones-img d-block">
							<picture >
							<source srcset="@/assets/img/iron.jpg" media="(max-width: 600px)" width="100%" height="auto"/>
							<img src="@/assets/img/iron.jpg" alt="Control system for your business" width="100%" height="auto"/>
						</picture>
							<ul class="d-md-none">
								<li><span>1.</span> Departments overview</li>
								<li><span>2.</span> personalized tickets</li>
								<li><span>3.</span> statisctics / performance</li>
							</ul>
						</div>
					</div>
					
				</div>
			</div>
		</TwoCols>
        <Contact/>
    </div>
    
</template>

<script>
import Intro from "@/components/Sections/Intro";
import TwoCols from "@/components/Sections/TwoCols";
import Contact from "@/components/Sections/Contact";
export default {
	components: {
        Intro,
        TwoCols,
		Contact
	},
    head() {
		return {
			bodyAttrs: {
				class: "header-transpar"
			}
		};
	}
};
</script>

<style lang="scss" scoped>
.wr {
    background: #F2F2F2;
}
.intro {
        background: #024751;
		min-height: 838px;
        // margin-bottom: 20rem;
        overflow: hidden;
		padding-bottom: 13.2rem !important;
        @include media-breakpoint-down(md) {
            margin-bottom: 0rem;
			padding-bottom: unset !important;
        
        }
        
        .intr-wrapp {
            padding-top: 27rem;
            position: relative;
            @include media-breakpoint-down(xl) {
                padding-top: 52rem;
            }
            h1 {
                font-size: 80px;
                line-height: 90px;
                max-width: 65rem;
                color: white;
				margin-bottom: 10rem;
                @include media-breakpoint-down(xl) {
                    font-size: 42px;
                    line-height: 50px;
					max-width: 100%;
					margin-bottom: 4rem;
                }
            }
			
			.intr-img-wrap {
				// margin-left: -2rem;
				// margin-right: -2rem;
			}
            .intr-img {
                position: absolute;
                top: 15rem;
                right: -30rem;
				@include media-breakpoint-down(xl) {
					right: -16rem;
					
					top: 3rem;
					
					// width: 100%;
					
					img {
						width: unset !important;
						margin: 0 auto;
					}
				}
            }
        }
		// min-height: calc(var(--vh, 1vh) * 92);
        
		@include media-breakpoint-up(md) {
			padding-bottom: 26.2rem;
			
		}
        @include media-breakpoint-down(md) {
            top: -5rem !important;
            
        }

		@include media-breakpoint-down(lg) {
			min-height: 812px;
            top: -10rem !important;
		}

		
	}
.two-cols-2 {
    padding-bottom: 8rem;
    @include media-breakpoint-up(lg) {
        padding-top: 20rem;
        padding-bottom: 16rem;
    }
    .img-holder {
        margin-bottom: 4rem;
        img {
            border-radius: 2.5rem;
        }
    }
    ul {
        @include media-breakpoint-up(md) {
            padding-bottom: 12rem;
        }
        
    }
    
}
.quick {
    padding-bottom: 17.5rem;
    @include media-breakpoint-down(md) {
        padding-bottom: 10rem;
    }
    .quick-wrap {
        max-width: 1190px;
        margin: 0 auto;
        background: white;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        padding: 8rem 3rem 0rem;
        border-radius: 20px;
        @include media-breakpoint-down(md) {
            padding: 3.2rem 2rem;
        }
    }
    .quick__item {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-transform: uppercase;
        width: 26rem;
        flex-wrap: wrap;
        p {
            margin-bottom: 0;
            @include media-breakpoint-down(md) {
                font-size: 1.8rem;
            }
        }
        &:not(:last-child){
            margin-bottom: 9rem;
            @include media-breakpoint-down(md) {
                margin-bottom: 3.2rem;
            }
        }
        img {
            margin-bottom: 1.6rem;
            @include media-breakpoint-down(md) {
            margin-bottom: 0;
            margin-right: 2rem;
            width: 4rem;
            height: 4rem;
        }
        
        }
        @include media-breakpoint-down(md) {
            flex-direction: row;
            width: 100%;
        }
    }
}

.phones {
		background: #F2F2F2;
		// padding-top: 20rem;
        padding-bottom: 18rem;
        border-radius: 0 0 4rem 4rem;
        margin-bottom: 16.2rem;
		@include media-breakpoint-down(lg) {
			padding-bottom: 5rem;
            border-radius: 0 0 2rem 2rem;
            margin-bottom: 8rem;
		}
		.two-col-h2 {
			margin-bottom: 6rem !important;
            font-size: 8rem;
            line-height: 90px;
			@include media-breakpoint-down(lg) {
                font-size: 4.2rem;
                line-height: 50px;
				margin-bottom: 3.2rem !important;
			}
			
		}
        .phones-span2 {
            margin-bottom: 4rem;
        }
		
		picture {
			max-width: 47rem !important;
		}
		ul {
			padding-left: 0 !important;
            max-width: 40rem;
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
					margin-bottom: 2.5rem;
				}
			}
		}
		.img-wrap {
			margin-top: 16rem;
			img {
				border-radius: 25px;
			}
			@include media-breakpoint-down(md) {
				margin-top: 5.5rem;
			}
		}
	}
</style>