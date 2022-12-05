<template>
	<transition>
		<div class="wrapper">
			<Header />
			<main class="main">
				<nuxt />
			</main>
			<Footer />
			<GoTopBtn />
		</div>
	</transition>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import globalBreakpoints from "@/mixins/globalBreakpoints";
import GoTopBtn from "@/components/Buttons/GoTopBtn";

export default {
	components: {
		Header,
		Footer,
		GoTopBtn
	},
	mixins: [globalBreakpoints]
};
</script>
