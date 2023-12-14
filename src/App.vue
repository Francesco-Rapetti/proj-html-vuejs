<script>
import AppNavbar from './components/AppNavbar.vue'
import PageHeader from './components/PageHeader.vue'
import PageSectionOne from './components/PageSectionOne.vue'
import PageSectionTwo from './components/PageSectionTwo.vue'
import PageSectionThree from './components/PageSectionThree.vue'
import PageSectionFive from './components/PageSectionFive.vue'
export default {
	components: {
		AppNavbar,
		PageHeader,
		PageSectionOne,
		PageSectionTwo,
		PageSectionThree,
		PageSectionFive
	}
}
</script>

<template>
	<header>
		<PageHeader />
	</header>

	<main>
		<PageSectionOne />
		<PageSectionTwo />
		<PageSectionThree />
		<PageSectionFive />
	</main>
</template>

<style scoped></style>
