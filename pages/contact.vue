<template>
	<div class="contact-page">
		<div class="container">
			<div class="row">
				<div class="col-md-6 d-flex flex-md-column flex-column-reverse">
					<h1 class="h1">Get in touch!</h1>
					<div class="place-img">
						<div class="img-holder">
							<img src="@/assets/images/img-018.png" alt="img phone" />
						</div>
					</div>
				</div>
				<div class="col-md-6">
					<div class="text-holder">
						<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consequat tellus pellentesque lorem aliquet. Etiam tempus aliquam at vitae venenatis mauris.</p>
					</div>
					<ContactForm />
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import ContactForm from "@/components/ContactForm";

export default {
	components: {
		ContactForm
	}
};
</script>

<style lang="scss" scoped>
.contact-page {
	position: relative;
	padding-top: 21rem;

	@include media-breakpoint-down(md) {
		padding-top: 4.5rem;
		padding-bottom: 6rem;
		overflow: hidden;
	}

	&::before {
		content: "";
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 80%;
		background: #d9d4ca;
		border-bottom-left-radius: 2rem;
		border-bottom-right-radius: 2rem;

		@include media-breakpoint-down(md) {
			border-bottom-left-radius: 1rem;
			border-bottom-right-radius: 1rem;
		}
	}

	.text-holder {
		margin-bottom: 9.4rem;
		color: rgba(black, 0.6);

		@include media-breakpoint-up(md) {
			padding-top: 1.5rem;
		}

		@include media-breakpoint-down(md) {
			margin-bottom: 4rem;
		}
	}

	.container {
		position: relative;
		z-index: 2;
	}

	.place-img {
		position: relative;

		.img-holder {
			@include media-breakpoint-up(md) {
				position: absolute;
				top: 5rem;
				left: 0;
				width: 116%;
			}

			@include media-breakpoint-down(md) {
				position: relative;
				right: -1rem;
				margin-right: -3rem;
				margin-bottom: 3rem;
			}

			img {
				width: 100%;
				height: auto;
			}
		}
	}
}
</style>
