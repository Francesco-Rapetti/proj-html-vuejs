<script>
import AppNavbar from './components/AppNavbar.vue'
import PageHeader from './components/PageHeader.vue'
import PageSectionOne from './components/PageSectionOne.vue'
export default {
	components: {
		AppNavbar,
		PageHeader,
		PageSectionOne,
	}
}
</script>

<template>
	<header>
		<PageHeader />
	</header>

	<main>
		<PageSectionOne />
	</main>
</template>

<style scoped></style>
