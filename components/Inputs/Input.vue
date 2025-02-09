<template>
	<div class="input-group" :class="{ focus: labelShow }">
		<label v-if="inputType === 'input'">
			<transition name="fade">
				<span v-if="(label && labelShow) || value.length > 0" class="label">{{ label }}</span>
			</transition>
			<input class="form-control" :type="type" :placeholder="placeholder" :value="value" v-on="listeners" @input="onInput" @focus="showHideLabel(true)" @blur="showHideLabel(false)" />
			<slot name="error">
				<span v-if="errorShowing" class="error-message"
					><span>{{ errorMessage }}</span></span
				>
			</slot>
		</label>
		<label v-if="inputType === 'textarea'">
			<transition name="fade">
				<span v-if="(label && labelShow) || value.length > 0" class="label">{{ label }}</span>
			</transition>
			<div class="textarea-holder">
				<textarea ref="textarea" class="form-control" :maxlength="maxlength" :placeholder="placeholder" :value="value" v-on="listeners" @input="onInput" @focus="showHideLabel(true)" @blur="showHideLabel(false)"></textarea>
				<span class="maxlength">
					{{ maxLength }}
				</span>
			</div>
			<slot name="error">
				<span v-if="errorShowing" class="error-message"
					><span>{{ errorMessage }}</span></span
				>
			</slot>
		</label>
	</div>
</template>

<script>
export default {
	name: "Input",
	props: {
		inputType: {
			type: String,
			default: "input"
		},
		type: {
			type: String,
			default: "text"
		},
		value: {
			type: String,
			default: ""
		},
		label: {
			type: String,
			default: ""
		},
		placeholder: {
			type: String,
			default: ""
		},
		errorMessage: {
			type: String,
			default: "Required field"
		},
		errorShowing: {
			type: Boolean,
			default: false
		},
		maxlength: {
			type: Number,
			default: 500
		}
	},
	data() {
		return {
			labelShow: false
		};
	},
	computed: {
		listeners() {
			const { input, ...rest } = this.$listeners;
			return rest;
		},

		maxLength() {
			return this.maxlength - this.value.length;
		}
	},
	methods: {
		onInput(value) {
			this.$emit("input", value.target.value);
		},
		onChange(value) {
			this.$emit("change", value.target.value);
		},
		showHideLabel(value) {
			this.labelShow = value;
		}
	}
};
</script>

<style lang="scss" scoped>
.input-group {
	position: relative;
	display: flex;
	flex-direction: column;
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
	}

	.form-control {
		padding: 1.6rem 3rem;
		font-size: 1.6rem;
		color: $black;
		border: 0.1rem solid rgba($black, 0.5);
		border-radius: 3rem;

		&::placeholder {
			color: rgba($black, 1);
		}

		@include media-breakpoint-down(md) {
			padding-left: 2rem;
			padding-right: 2rem;
			font-size: 1.4rem;
		}

		&:focus {
			box-shadow: none;
		}
	}

	.textarea-holder {
		position: relative;

		.maxlength {
			position: absolute;
			right: 1.5rem;
			bottom: 1.5rem;
			font-size: 1rem;
			color: rgba($black, 0.5);
		}
	}

	textarea {
		min-height: 11.5rem;
		resize: none;
	}

	.error-message {
		// position: absolute;
		// left: 0;
		// bottom: -2rem;
		font-size: 1.4rem;
		color: $red;

		@include media-breakpoint-down(md) {
			// bottom: -1.6rem;
			font-size: 1.2rem;
		}
	}

	// &.focus {
	// 	.label {
	// 		color: black;
	// 	}
	// }
}
</style>
