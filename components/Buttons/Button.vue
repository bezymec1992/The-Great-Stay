<template>
	<nuxt-link v-if="type === 'nuxt-link'" :to="to" class="btn" :class="hasIconSlot === false ? 'd-inline-block' : null" :style="style"
		>{{ title }}
		<span v-if="hasIconSlot" class="icon-holder">
			<slot name="icon" />
		</span>
	</nuxt-link>
	<a v-else-if="type === 'link'" :href="href" target="_blank" class="btn" :class="hasIconSlot === false ? 'd-inline-block' : null" :style="style"
		>{{ title }}

		<span v-if="hasIconSlot" class="icon-holder">
			<slot name="icon" />
		</span>
	</a>
	<button v-else-if="type === 'button'" class="btn" :class="hasIconSlot === false ? 'd-inline-block' : null" :style="style" @click="click">
		{{ title }}

		<span v-if="hasIconSlot" class="icon-holder">
			<slot name="icon" />
		</span>
	</button>
</template>

<script>
export default {
	name: "Button",
	props: {
		type: {
			type: String,
			default: "button",
			require: false
		},
		title: {
			type: String,
			default: "title",
			require: false
		},
		to: {
			type: [String, Object],
			default: ""
		},
		href: {
			type: String,
			default: "#",
			require: false
		},
		color: {
			type: String,
			default: "black"
		},
		backgroundColor: {
			type: String,
			default: "white"
		}
	},
	data() {
		return {
			style: {
				"--color": this.color,
				"--background-color": this.backgroundColor
			}
		};
	},
	computed: {
		hasIconSlot() {
			return !!this.$slots.icon;
		}
	},
	methods: {
		click() {
			this.$emit("click");
		}
	}
};
</script>

<style lang="scss" scoped>
.btn {
	display: inline-flex;
	justify-content: space-between;
	align-items: center;
	padding: 1.9rem 4rem;
	font-size: 1.8rem;
	line-height: 1;
	color: var(--color);
	letter-spacing: 0.1rem;
	background: var(--background-color);
	border: solid 0.1rem var(--background-color);
	border-radius: 3rem;

	@include media-breakpoint-down(md) {
		padding: 1.7rem 2.6rem;
		font-size: 1.6rem;
	}

	&:focus {
		box-shadow: none;
	}

	.icon-holder {
		display: inline-flex;
		margin-left: 1.6rem;

		@include media-breakpoint-down(md) {
			margin-left: 1.3rem;
		}
	}

	&.btn-dark {
		color: $white;
		background: $black;
		border-color: $black;

		&:hover {
			background: lighten($black, 10);
			border-color: lighten($black, 10);
		}
	}

	&.btn-outline-dark {
		color: $black;
		background: transparent;
		border-color: $black;
		width: 100%;
		font-size: 18px;
		text-transform: unset !important;
		&:hover {
			color: $white;
			background: $black;
			border-color: $black;
		}
	}

	&.btn-light {
		color: $black;
		background: $white;
		border-color: $white;

		&:hover {
			color: $black;
			background: darken($white, 10);
			border-color: darken($white, 10);
		}
	}
}
</style>
