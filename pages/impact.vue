<template>
    <div>
        <Intro>
			<div class="container">
				<div class="row flex-column-reverse flex-md-row">
					<!-- <div class="col-md-8">
						<div class="content-holder">
							<h1 class="h1">
								
							</h1>
							
						</div>
					</div> -->
					<div class="col">
						<div class="background"></div>
						<!-- <picture class="img-holder">
							<source srcset="@/assets/images/img-02.jpg" media="max-widtn: 575px" />
							<img src="@/assets/images/img-01.jpg" alt="Control system for your business" />
						</picture> -->
					</div>
				</div>
			</div>
		</Intro>

        <Contact/>
    </div>
    
</template>

<script>
import Intro from "@/components/Sections/Intro";
import Contact from "@/components/Sections/Contact";
export default {
	components: {
        Intro,
		Contact
	}
};
</script>

<style lang="scss" scoped>

</style>