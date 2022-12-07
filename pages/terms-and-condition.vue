<template>
	<div class="privacy-policy">
		<div class="container">
			<div class="text-holder">

                <h1 class="privacy__title">Terms and Conditions</h1>
            <p class="privacy-text">
                1.By accessing this website and any of its associated websites or mobile applications (the “Site”), you acknowledge these terms and conditions of use and agree to be bound by them. If you do not agree to these terms, please discontinue accessing the Site immediately.
            </p>
            <p class="privacy-text">
                2. We reserve the right, in our sole discretion, to modify, alter or otherwise update these terms and conditions at any time and you agree to be bound by such modifications, alterations or updates.
            </p>
            <p class="privacy-text">
                3.The content of the Site is published by Great Stay and its affiliates.
            </p>
            <p class="privacy-text">
                4.This Site is only intended to provide you with general information and is neither an offer to sell nor a solicitation of an offer to purchase any security and may not be relied upon for investment purposes.
            </p>
            <p class="privacy-text">
                5.Any commentaries and information contained in the Site should not be considered personal investment advice.
            </p>
            <p class="privacy-text">
                6.Information on the Site is not intended to provide legal, accounting, financial or tax advice, and should not be relied upon in that regard. Please consult with your professional advisor with respect to your particular circumstances.
            </p>
            <p class="privacy-text">
                7.The Site is provided on an “as is” and “as available” basis, without any representations, warranties or conditions of any kind, whether expressed or implied, and including without limitation implied representations, warranties or conditions of title, non-infringement, merchantability, fitness for a particular purpose, performance, durability, availability, timeliness, accuracy, or completeness, all of which are hereby disclaimed by Wealthsimple to the fullest extent permitted by law.
            </p>
            <p class="privacy-text">
                8.Every effort has been made to ensure that the material contained on the site is accurate at the time of publication. However, Great Stay will not under any circumstances be liable to you or any other person in any way for any loss or damages (direct, indirect, special, economic, incidental, consequential, punitive or exemplary, including without limitation loss of revenue, data, anticipated profits or lost business) in respect of use of, or inability to use, or any reliance on, the Site, any of its content or links (including without limitation any inaccuracies or viruses), or any web browser or other equipment.
            </p>
            <p class="privacy-text">
                9.By accessing the Site, you agree to indemnify and hold harmless Great Stay and its agents, suppliers and their respective directors, officers and employees from and against any and all actions, proceedings, costs, claims, liabilities, damages and expenses (including reasonable legal fees) arising from or in connection with a breach of these terms and conditions or the use of this Site.
            </p>
            <p class="privacy-text">
                10.The contents of the Site are protected by applicable copyright and trademark laws. Unauthorized use or exploitation of such content is strictly prohibited including without limitation, unauthorized downloading, retransmission, storage in any medium, copying, redistribution, reproduction, or republication of the Site, or any part thereof, for any purpose.
            </p>
            <p class="privacy-text">
                11.Other sites accessed by hypertext appearing in the Site may have been independently developed by parties other than Great Stay. Great Stay does not guarantee the accuracy of information contained in such other sites.
            </p>
            <p class="privacy-text">
                12.Links to other sites should not be taken as Great Stay`s endorsement or approval of such other sites, the third parties named therein, or their products and services, nor is any liability assumed for incompatibility, non-suitability, viral infection or other destructive/disruptive components on or from such other sites.
            </p>
            <p class="privacy-text">
                13.The framing, mirroring, scraping or data-mining of the Site or any of its content in any form and by any method is strictly prohibited.
            </p>
            <p class="privacy-text">
                14.Great Stay cannot guarantee complete confidentiality or security for information that is transmitted electronically. By accessing the Site, you acknowledge that Great Stay is not responsible for any damages or losses you may suffer as a result of your electronic transmission of confidential or sensitive information to us. Please refer to Great Stay`s privacy policy for more information.
            </p>
            <p class="privacy-text">
                15.No consent or waiver by either party to, or of any breach or default by, the other party in its performance of its obligations under this agreement will be deemed or construed to be a consent to, or a waiver of, a continuing breach or default or any other breach or default of those or any other obligations of that party. No consent or waiver will be effective unless in writing.
            </p>
            <p class="privacy-text">
                16.If any provision of these terms and conditions is found to be unlawful, void, or for any reason unenforceable, then that provision shall be deemed to be severed from the rest of these terms and conditions and shall not affect the validity and enforceability of any remaining provisions.
            </p>
            <p class="privacy-text">
                17.These terms and conditions are governed by the laws of State of Delaware and the laws of the United States applicable therein, excluding any conflict of laws which would lead to the application of any other laws. By accessing the Site, you hereby irrevocably submit and attorn to the provincial and federal courts located in the State of Delaware, for any disputes or matters arising from, connected with, or relating to the Site, this agreement or any related matters.
            </p>
            </div>
		</div>
	</div>
</template>

<script>
export default {
	head() {
		return {
			bodyAttrs: {
				class: "footer-has-pt header-white-bg"
			}
		};
	}
};
</script>

<style lang="scss" scoped>
.privacy-policy {
	padding-top: 20rem;
	padding-bottom: 4.3rem;
	@include media-breakpoint-down(md) {
		padding-top: 5.1rem;
		padding-bottom: 10rem;
	}
	.privacy-wrapp {
		justify-content: space-between;
		display: flex;
		margin-top: 7rem;
		@include media-breakpoint-down(md) {
			display: block !important;
			margin-top: 4rem;
		}
	}
	.privacy-subtitle {
		max-width: 40rem;
		width: 100%;
		font-weight: 400;
		font-size: 30px;
		line-height: 40px;
		@include media-breakpoint-down(md) {
			font-size: 26px;
			line-height: 31px;
			margin-bottom: 2.3rem;
		}		
	}

    .privacy-text {
        font-size: 1.8rem;
        line-height: 28px;
        font-weight: 400;
        @include media-breakpoint-down(md) {
			font-size: 14px;
			line-height: 22px;
		}
    }

	.privacy__title {
		margin-bottom: 6rem;
		font-weight: 400;
		font-size: 72px;
		line-height: 104px;

		@include media-breakpoint-down(md) {
			margin-bottom: 3.5rem;
			font-size: 40px;
			line-height: 48px;
		}
	}

	.text-holder {
		@include media-breakpoint-down(md) {
			font-size: 1.4rem;
		}

		p {
			&:not(:last-child) {
				margin-bottom: 4rem;

				@include media-breakpoint-down(md) {
					margin-bottom: 3rem;
				}
			}
		}

		a {
			color: black;
			// text-decoration: underline;

			&:hover {
				text-decoration: none;
			}
		}
	}
}
</style>
