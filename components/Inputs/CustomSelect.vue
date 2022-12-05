<template>
	<div class="custom-select-wrapper">
		<div class="custom-select" :tabindex="tabindex" @blur="open = false">
			<span v-if="label" class="label">{{ label }}</span>
			<div class="selected" :class="[{ open: open }, !selected.title ? 'no-selected' : '']" @click="open = !open">
				{{ !selected.title ? this.default : selected.title }}
			</div>
			<div class="select-items" :class="{ selectHide: !open }" @click="clicked">
				<div
					v-for="(option, i) of options"
					:key="i"
					@click="
						selected = option;
						open = false;
					"
					class="select-item"
				>
					{{ option.title }}
				</div>
			</div>
		</div>
		<span v-if="errorShowing" class="error-message"
			><span>{{ errorMessage }}</span></span
		>
	</div>
</template>

<script>
export default {
	props: {
		options: {
			type: Array,
			required: true,
			default: () => []
		},
		default: {
			type: String,
			required: false,
			default: null
		},
		tabindex: {
			type: Number,
			required: false,
			default: 0
		},
		errorShowing: {
			type: Boolean,
			default: false
		},
		errorMessage: {
			type: String,
			required: false,
			default: null
		},
		label: {
			type: String,
			default: ""
		},
		value: {
			type: [String, Object],
			default: ""
		}
	},
	data() {
		return {
			selected: this.default ? this.default : this.options.length > 0 ? this.options[0] : null,
			open: false
		};
	},
	// methods() {
	// 	this.$emit("input", this.selected);
	// },
	methods: {
		clicked() {
			this.$emit("input", this.selected.value);
		}
	}
};
</script>

<style lang="scss" scoped>
.custom-select-wrapper {
	margin-bottom: 1.5rem;

	@include media-breakpoint-down(md) {
		margin-bottom: 2.4rem;
	}

	.error-message {
		font-size: 1.4rem;
		color: $red;

		@include media-breakpoint-down(md) {
			font-size: 1.2rem;
		}
	}
}

.custom-select {
	position: relative;

	font-size: 1.6rem;
	cursor: pointer;

	@include media-breakpoint-down(md) {
		font-size: 1.4rem;
	}

	.label {
		display: block;
		margin-bottom: 1.2rem;
		font-size: 2rem;
		line-height: 1;

		@include media-breakpoint-down(md) {
			margin-bottom: 1rem;
			font-size: 1.6rem;
		}
	}

	.selected {
		display: flex;
		justify-content: space-between;
		padding: 1.7rem 3rem;
		align-items: center;
		color: $black;
		user-select: none;
		border: solid 0.1rem rgba($black, 0.5);
		border-radius: 3rem;
		transition: all 0.1s linear;

		@include media-breakpoint-down(md) {
			padding-left: 2rem;
			padding-right: 2rem;
		}

		&:after {
			content: "";
			right: 3rem;
			min-width: 1.6rem;
			width: 1.6rem;
			height: 0.8rem;
			background: url("data:image/svg+xml,%3Csvg width='18' height='10' viewBox='0 0 18 10' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 1L9 9L17 1' stroke='black'/%3E%3C/svg%3E%0A") no-repeat;
			background-size: 1.6rem;
			transition: all 0.1s linear;
		}

		&.no-selected {
			color: $black;
		}

		&.open {
			border-bottom-right-radius: 0;
			border-bottom-left-radius: 0;

			&:after {
				transform: rotate(180deg);
			}
		}
	}

	.select-items {
		overflow: hidden;
		position: absolute;
		left: 0;
		top: 100%;
		width: 100%;
		background-color: $white;
		z-index: 1;
		transition: all 0.1s linear;
		border-bottom-left-radius: 3rem;
		border-bottom-right-radius: 3rem;
		border-right: solid 0.1rem rgba($black, 0.5);
		border-left: solid 0.1rem rgba($black, 0.5);

		&.selectHide {
			opacity: 0;
			visibility: hidden;
			pointer-events: none;
		}
	}

	.select-item {
		padding: 1.7rem 3rem;
		border-bottom: solid 0.1rem rgba($black, 0.5);
		transition: all 0.1s linear;

		&:hover {
			background: rgba($black, 0.05);
		}
	}
}
</style>
