<template>
	<header class="header">
		<div class="container">
			<strong class="logo">
				<nuxt-link to="/">Logo</nuxt-link>
			</strong>

			<nav class="main-nav">
				<ul class="main-menu">
					<li v-for="(item, index) in menu" :key="index" @click="closeMenu">
						<nuxt-link :to="item.to">{{ item.title }}</nuxt-link>
					</li>
				</ul>
			</nav>
			<a class="open-menu d-lg-none" :class="{ open: menuOpen }" href="#" @click.prevent="toggleMenu">
				<span></span>
				<span></span>
				<span class="visually-hidden">Open Mobile Nav</span>
			</a>
		</div>
	</header>
</template>

<script>
export default {
	name: "Header",
	data() {
		return {
			menuOpen: false,
			menu: [
				{
					title: "impact",
					to: "/modules"
				},
				{
					title: "Your place",
					to: "/crm-cms"
				},
				{
					title: "for customers",
					to: "/app"
				},
				{
					title: "Contact",
					to: "/contact"
				}
			]
		};
	},
	methods: {
		toggleMenu() {
			this.menuOpen = !this.menuOpen;

			if (this.menuOpen) {
				document.body.classList.add("menu-opened");
			} else {
				document.body.classList.remove("menu-opened");
			}
		},
		closeMenu() {
			this.menuOpen = false;
			document.body.classList.remove("menu-opened");
		}
	}
};
</script>

<style lang="scss" scoped>
.header {
	padding-top: 3.8rem;
	padding-bottom: 3.8rem;
	z-index: 100;
	color: white;
	@include media-breakpoint-down(lg) {
		padding-top: 3.2rem;
		padding-bottom: 3.2rem;
		color: black;
	}

	@include media-breakpoint-down(md) {
		background: $white;
	}

	@include media-breakpoint-up(lg) {

		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
	}

	.header-white-bg & {
		background: white;
	}

	> .container {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.logo {
		font-weight: 400;
		font-size: 2.4rem;
		text-transform: uppercase;
	}

	.main-nav {
		text-transform: uppercase;
		transition: $transition;

		@include media-breakpoint-down(lg) {
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			display: flex;
			padding: 10.3rem 3rem 8rem 3rem;
			background: $white;
			opacity: 0;
			visibility: hidden;
			pointer-events: none;
			z-index: 99;
		}

		.menu-opened & {
			@include media-breakpoint-down(lg) {
				opacity: 1;
				visibility: visible;
				pointer-events: all;
			}
		}

		.main-menu {
			margin: 0;
			padding: 0;
			list-style: none;

			@include media-breakpoint-down(lg) {
				width: 100%;
				overflow: auto;
				text-align: center;
			}

			@include media-breakpoint-up(lg) {
				display: flex;
			}

			li {
				&:not(:last-child) {
					@include media-breakpoint-up(lg) {
						margin-right: 4rem;
					}

					@include media-breakpoint-up(xxl) {
						margin-right: 7rem;
					}

					@include media-breakpoint-down(lg) {
						margin-bottom: 8.1rem;
					}
				}
			}

			a {
				position: relative;
				&::after {
					content: "";
					position: absolute;
					width: 100%;
					transform: scaleX(0);
					height: 0;
					bottom: -0.3rem;
					left: 0;
					border-bottom: 0.2rem solid;
					transform-origin: bottom right;
					transition: transform 0.25s ease-out;
				}

				

				&:hover {
					&::after {
						transform: scaleX(1);
						transform-origin: bottom left;
					}
				}
				&.nuxt-link-exact-active {
        			&::after {
          				transform: scaleX(1);
          				transform-origin: bottom left;
        			}
      			}
			}
		}
	}

	.open-menu {
		position: relative;
		width: 3rem;
		height: 3rem;
		display: block;
		font-size: 0;
		line-height: 0;
		z-index: 100;

		span {
			position: absolute;
			top: 50%;
			left: 0;
			width: 100%;
			border-bottom: 0.3rem solid;
			height: 0;
			transition: $transition;

			// .menu-opened & {
			// 	@include media-breakpoint-down(lg) {
			// 		color: $white;
			// 	}
			// }

			&:nth-child(1) {
				margin-top: -0.5rem;

				.menu-opened & {
					margin-top: 0;
					transform: rotate(45deg);
				}
			}

			&:nth-child(2) {
				margin-top: 0.5rem;

				.menu-opened & {
					margin-top: 0;
					transform: rotate(-45deg);
				}
			}
		}
	}
}
</style>
