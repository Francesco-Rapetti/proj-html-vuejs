<script>
import AppNavbar from './components/AppNavbar.vue'
import PageHeader from './components/PageHeader.vue'
import PageSectionOne from './components/PageSectionOne.vue'
import PageSectionTwo from './components/PageSectionTwo.vue'
export default {
	components: {
		AppNavbar,
		PageHeader,
		PageSectionOne,
		PageSectionTwo
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
	</main>
</template>

<style scoped></style>
