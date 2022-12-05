<template>
	<div class="phone-input">
		<label>
			<transition name="fade">
				<span v-if="(label && labelShow) || (value && value.length > 0)" class="label">{{ label }}</span>
			</transition>
			<VuePhoneNumberInput :value="value" :border-radius="30" maxlength="17" :translations="{ phoneNumberLabel: 'Your phone' }" v-on="listeners" @input="onInput" @update="results = $event" @focus="showHideLabel(true)" @blur="showHideLabel(false)" />
			<slot name="error">
				<span v-if="errorShowing" class="error-message"
					><span>{{ errorMessage }}</span></span
				>
			</slot>
		</label>
	</div>
</template>

<script>
import VuePhoneNumberInput from "vue-phone-number-input";
import "vue-phone-number-input/dist/vue-phone-number-input.css";

export default {
	name: "PhoneInput",
	components: {
		VuePhoneNumberInput
	},
	model: {
		event: "input",
		prop: "value"
	},
	props: {
		label: {
			type: String,
			default: ""
		},
		value: {
			type: [Object, String],
			default: () => ({})
		},
		errorMessage: {
			type: String,
			default: "Required field"
		},
		errorShowing: {
			type: Boolean,
			default: false
		}
	},
	data() {
		return {
			results: {},
			labelShow: false
		};
	},
	computed: {
		listeners() {
			const { input, ...rest } = this.$listeners;
			return rest;
		}
	},
	methods: {
		onInput(value) {
			this.$emit("input", value);
		},
		showHideLabel(value) {
			this.labelShow = value;
		}
	}
};
</script>

<style lang="scss" scoped>
.phone-input {
	margin-bottom: 1.5rem;

	label {
		width: 100%;
	}

	.label {
		position: absolute;
		top: 0;
		left: 2rem;
		transform: translateY(-50%);
		display: block;
		padding: 0.1rem 1rem;
		font-size: 1.6rem;
		color: rgba($black, 0.5);
		background: white;
		z-index: 2;

		@include media-breakpoint-down(md) {
			font-size: 1.4rem;
		}
	}

	.error-message {
		// position: absolute;
		font-size: 1.4rem;
		color: $red;

		@include media-breakpoint-down(md) {
			font-size: 1.2rem;
		}
	}
}
</style>

<style lang="scss">
.phone-input {
	position: relative;

	.vue-phone-number-input {
		.select-country-container {
			max-width: 100%;
			width: 100%;
		}
	}

	.country-selector {
		min-height: 5.6rem;
		height: 5.6rem;

		input {
			color: black;
			border-color: rgba($black, 0.5) !important;
		}
	}

	.country-selector__toggle {
		pointer-events: none;
	}

	.country-selector__input {
		min-height: 5.6rem;
		height: 5.6rem;
		box-shadow: none !important;
	}

	.input-tel__input {
		color: black;
		min-height: 5.6rem;
		height: 5.6rem;
		box-shadow: none !important;

		&::placeholder {
			color: black;
		}
	}

	.input-tel {
		min-height: 5.6rem;
		height: 5.6rem;

		input {
			border-color: rgba($black, 0.5) !important;
		}
	}

	.country-selector__country-flag {
		top: 29px;
		left: 14px;
	}

	.country-selector__label {
		top: 9px;
		left: 14px;
	}
}
</style>
