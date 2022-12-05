<template>
	<footer class="footer">
		<div class="container">
			<div class="left-side">
				<strong class="logo">Logo</strong>
				<address class="address">
					<p>
						Netherlands 12762 <br />
						S. Zholtogo st, 62 <br />
						office 16<br /><br />
						<a href="tel:+175 22 426 22">+175 22 426 22</a>
					</p>
				</address>
				<SocialLinks />
			</div>
			<div class="right-side">
				<div class="row">
					<div class="col-md-6">
						<div class="menus-holder">
							<ul class="menu">
								<li v-for="(link, index) in links.slice(0, 3)" :key="index">
									<nuxt-link :to="link.route">{{ link.title }}</nuxt-link>
								</li>
							</ul>
							<ul class="menu">
								<li v-for="(link, index) in links.slice(3, links.length)" :key="index">
									<nuxt-link :to="link.route">{{ link.title }}</nuxt-link>
								</li>
							</ul>
						</div>
					</div>
					<div class="col-md-6 d-flex align-items-md-end">
						<div class="copyright">
							
							<p class="mb-0 text-capitalize">&copy;all rights reserved</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</footer>
</template>

<script>
import SocialLinks from "@/components/SocialLinks";

export default {
	name: "Footer",
	components: {
		SocialLinks
	},
	data() {
		return {
			links: [
				{
					title: "Home",
					route: "/crm-cms"
				},
				{
					title: "impact",
					route: "/app"
				},
				
				{
					title: "Your place",
					route: "/contact"
				},
				{
					title: "contact",
					route: "/contact"
				},

				{
					title: "PRIVACY POLICY ",
					route: "/privacy-policy"
				},
				{
					title: "TERMS AND CONDITIONS",
					route: "/"
				}
			]
		};
	}
};
</script>

<style lang="scss" scoped>
.footer {
	padding-bottom: 20rem;
	font-size: 2rem;

	@include media-breakpoint-down(md) {
		padding-bottom: 8rem;
	}

	.footer-has-pt & {
		padding-top: 18rem;

		@include media-breakpoint-down(md) {
			padding-top: 6.2rem;
		}
	}

	a {
		&:hover {
			opacity: 0.7;
		}
	}

	.container {
		@include media-breakpoint-up(md) {
			display: flex;
		}
	}

	.left-side {
		margin-right: 10rem;
	}

	.right-side {
		width: 100%;
	}

	.logo {
		display: block;
		margin-bottom: 3rem;
		font-weight: 400;
		font-size: 2.4rem;
		line-height: 1;
		text-transform: uppercase;

		@include media-breakpoint-down(md) {
			margin-bottom: 4rem;
		}
	}

	.address {
		margin-bottom: 5.6rem;

		@include media-breakpoint-down(md) {
			margin-bottom: 4.2rem;
		}
	}

	.menus-holder {
		padding-top: 5.2rem;

		@include media-breakpoint-down(md) {
			display: flex;
			padding-top: 4.2rem;
		}

		.menu {
			&:first-child {
				@include media-breakpoint-down(md) {
					margin-right: 3rem;
				}
			}

			&:last-child {
				li {
					&:last-child {
						margin-bottom: 0;
					}
				}
			}
		}
	}

	.menu {
		margin: 0;
		padding: 0;
		list-style: none;

		@include media-breakpoint-down(md) {
			font-size: 1.8rem;
		}

		li {
			margin-bottom: 2.6rem;
			text-transform: uppercase;
			@include media-breakpoint-down(md) {
				margin-bottom: 2rem;
			}
		}
	}

	.copyright {
		@include media-breakpoint-down(md) {
			font-size: 1.4rem;
		}
	}
}
</style>
