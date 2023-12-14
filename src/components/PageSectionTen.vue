<script>
import AppCarouselThree from './AppCarouselThree.vue';
export default {
    components: {
        AppCarouselThree
    }
}
</script>

<template>
    <div class="wrapper">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <p class="highlight">Latest News</p>
                    <h1 class="title">Stay Updated With out Latest News Articles</h1>
                </div>
            </div>

            <AppCarouselThree />
        </div>
    </div>
</template>

<style scoped>
.wrapper {
    height: 950px;
    display: flex;
    align-items: center;
    padding-bottom: 150px;
}
</style>