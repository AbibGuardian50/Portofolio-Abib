<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						"Hi, You can call me Abib, has experience in front-end development using Vue.js and software quality assurance with automation tools like Katalon. Although my experience is still growing, I'm eager to learn new things and always strive to give my best in every project,I enjoy working in a team and love the challenge of finding the best solutions. My education and experience shaped required skills in front-end development and software quality assurance.If you're looking for someone who's enthusiastic and dedicated, feel free to reach out",
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
