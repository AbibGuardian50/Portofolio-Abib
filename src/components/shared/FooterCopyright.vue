<script>
export default {
	data: () => {
		return {
			copyrightDate: new Date().getFullYear(),
			author: 'Abib',
		};
	},
};
</script>

<template>
	<div class="flex justify-center items-center text-center">
		<div class="font-general-regular text-lg text-ternary-dark dark:text-ternary-light">
			&copy; {{ copyrightDate }}.
			Visit me on Github
			<a href="https://github.com/AbibGuardian50" target="__blank"
				class="font-general-medium text-secondary-dark dark:text-secondary-light uppercase hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500">{{
					author }}</a>
		</div>
	</div>
</template>

<style lang="scss" scoped></style>
