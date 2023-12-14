<script>
import AppNavbar from './components/AppNavbar.vue'
import PageHeader from './components/PageHeader.vue'
import PageSectionOne from './components/PageSectionOne.vue'
import PageSectionTwo from './components/PageSectionTwo.vue'
import PageSectionThree from './components/PageSectionThree.vue'
import PageSectionFive from './components/PageSectionFive.vue'
import PageFooter from './components/PageFooter.vue'
export default {
	components: {
		AppNavbar,
		PageHeader,
		PageSectionOne,
		PageSectionTwo,
		PageSectionThree,
		PageSectionFive,
		PageFooter
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
		<PageFooter />
	</main>
</template>

<style scoped></style>
