<template>
	<div class="contact-section">
		<div class="container">
			<div class="row">
				<div class="col-md-5">
					<h2 class="h2">Get in touch</h2>
					<div class="text-holder">
						<p>What to know more or be a part of the Great Stay? Then do not hesitate to contact us!</p>
					</div>
				</div>
				<div class="col-md-7">
					<ContactForm />
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import ContactForm from "@/components/ContactForm";
export default {
	components: { ContactForm }
};
</script>

<style lang="scss" scoped>
.contact-section {
	position: relative;
	padding-top: 12rem;
	padding-bottom: 6rem;

	@include media-breakpoint-down(md) {
		padding-top: 8rem;
		padding-bottom: 6rem;
	}

	&::before {
		content: "";
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 80%;
		background: #014751;
		border-bottom-left-radius: 2rem;
		border-bottom-right-radius: 2rem;

		@include media-breakpoint-down(md) {
			border-bottom-left-radius: 1rem;
			border-bottom-right-radius: 1rem;
		}
	}

	.container {
		position: relative;
		z-index: 2;
	}

	.h2 {
		margin-bottom: 4rem;
		color: white;
		font-size: 74px;
		line-height: 94px;
		@include media-breakpoint-down(md) {
			font-size: 50px;
			line-height: 60px;
			margin-bottom: 2rem;
		}
	}

	.text-holder {
		max-width: 42rem;
		color: #FFFFFF;
		opacity: 0.6;

		font-weight: 400;
		font-size: 28px;
		line-height: 36px;
		@include media-breakpoint-down(md) {
			margin-bottom: 4rem;
			
			font-size: 22px;
			line-height: 30px;
			
		}
	}
}
</style>
