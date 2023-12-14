<script>
import AppCarouselTwo from './AppCarouselTwo.vue';
export default {
    components: {
        AppCarouselTwo
    }
}
</script>

<template>
    <div class="wrapper">
        <div class="filter"></div>
        <div class="container position-relative z-index-1">
            <div id="content" class="w-100">
                <div class="w-50">
                    <p class="highlight">Trending Games</p>
                    <h1 class="title">Choose Who Is The Best In The World!</h1>
                </div>
                <AppCarouselTwo />
            </div>
        </div>
    </div>
</template>

<style scoped>
#content {
    padding: 120px 0;
}

.filter {
    position: absolute;
    width: inherit;
    height: inherit;
    background-color: #2020466d;
}

.wrapper {
    width: 100%;
    height: 816px;
    background-image: url('../assets/img/protfolio-vector.png');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>