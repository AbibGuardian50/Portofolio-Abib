<script>
import feather from 'feather-icons';
import ContactDetails from '@/components/contact/ContactDetails.vue';

export default {
	components: {
		ContactDetails,
	},
	data: () => {
		return {
			contacts: [
				{
					id: 1,
					name: 'Muhammad Abieb Basnuril',
					icon: 'linkedin',
					url: "https://www.linkedin.com/in/muhammad-abieb-basnuril/"
				},
				{
					id: 2,
					name: 'banurilabib@gmail.com',
					icon: 'mail',
					url: "mailto:banurilabib@gmail.com"
				},
			],
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div
		class="container mx-auto flex flex-col-reverse md:flex-row py-5 md:py-10 md:mt-10"
	>

		<!-- Contact details -->
		<ContactDetails :contacts="contacts" />
	</div>
</template>
