<template>
    <div class="wr">
        <Intro>
			<div class="container">
				<div class="intr-wrapp">
                
                    <h1>Provide the best experience for your customers</h1>
					<!-- <div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								
							</h1>
							
						</div>
					</div> -->
					<div class="intr-img">
						<!-- <div class="background"></div> -->
						<!-- <picture class="img-holderr">
							<source srcset="@/assets/img/place-dd.png" media="max-widtn: 575px" width="100%" height="auto"/>
							<img src="@/assets/img/place-mm.png" alt="Control system for your business" width="100%" height="auto" />
						</picture> -->
					</div>
				</div>
			</div>
		</Intro>
        <Contact />
    </div>
</template>

<script>
import Intro from "@/components/Sections/Intro";
import Contact from "@/components/Sections/Contact";
export default { 
	components: {
		Intro,
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

.intro {
        background: #024751;
		min-height: 838px;
        margin-bottom: 10rem;
        overflow: hidden;
        
        .intr-wrapp {
            padding-top: 27rem;
            position: relative;
            h1 {
                font-size: 80px;
                line-height: 90px;
                max-width: 65rem;
                color: white;
            }
            .intr-img {
                position: absolute;
                top: 10rem;
                right: -20rem;
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
            
			// min-height: calc(100vh - 8rem);
			// min-height: calc(var(--vh, 1vh) * 100 - 8rem);
			// padding-bottom: 8rem;
			// background: linear-gradient(90deg, #f4f4f4 0%, #f1f1f1 42.19%, #e8e7e5 100%);

			// h1 {
			// 	font-size: 4.8rem;
			// 	margin-bottom: 3rem;
			// 	line-height: 5rem;
			// }
		}

		// .background {
		// 	@include media-breakpoint-up(md) {
		// 		position: absolute;
		// 		top: 0;
		// 		left: 0;
		// 		width: 100%;
		// 		height: 100%;
		// 		background: url("@/assets/img/place-d.jpg") no-repeat;
		// 		background-size: cover;
		// 		background-position: center;
		// 	}

		// 	@include media-breakpoint-down(md) {
		// 		margin-left: -2rem;
		// 		margin-right: -2rem;
		// 		min-height: 73.2rem;
		// 		background: url("@/assets/img/place-m.jpg") no-repeat;
		// 		background-size: cover;
		// 		background-position: center;
		// 	}

		// 	img {
		// 		width: 100%;
		// 		height: auto;

		// 		@include media-breakpoint-up(md) {
		// 			height: 100%;
		// 			// object-fit: cover;
		// 		}
		// 	}
		// }

		// .content-holder {
		// 	@include media-breakpoint-down(md) {
		// 		padding-top: 3.4rem;
		// 	}
		// }
	}
</style>