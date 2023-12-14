<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation } from 'swiper/modules';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';
export default {
    name: 'AppCarousel',

    components: {
        Swiper,
        SwiperSlide,
    },


    props: {
        type: String,
        slidesPerView: Number,
    },

    setup() {
        return {
            modules: [Navigation],
        };
    },
}
</script>

<template>
    <div class="carousel position-relative">

        <Swiper :modules="modules" :slides-per-view="slidesPerView" :space-between="20" :loop="true"
            :navigation="{ nextEl: '.btn-next', prevEl: '.btn-prev' }">
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/v-small1.png" alt="">
                    </div>
                    <p class="title">Call Of Deauty</p>
                    <p class="text">Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui.</p>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/v-small2.png" alt="">
                    </div>
                    <p class="title">Assaaain Creed</p>
                    <p class="text">Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui.</p>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/v-small1.png" alt="">
                    </div>
                    <p class="title">Call Of Deauty</p>
                    <p class="text">Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui.</p>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/v-small2.png" alt="">
                    </div>
                    <p class="title">Assaaain Creed</p>
                    <p class="text">Vestibulum ac diam sit amet quam vehicula elementum sed sit amet
                        dui.</p>
                </div>
            </SwiperSlide>

        </Swiper>
        <div class="button btn-next">
            <svg class="svg-inline--fa fa-arrow-right-long" aria-hidden="true" focusable="false" data-prefix="fas"
                data-icon="arrow-right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                data-fa-i2svg="">
                <path fill="currentColor"
                    d="M502.6 278.6l-128 128c-12.51 12.51-32.76 12.49-45.25 0c-12.5-12.5-12.5-32.75 0-45.25L402.8 288H32C14.31 288 0 273.7 0 255.1S14.31 224 32 224h370.8l-73.38-73.38c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0l128 128C515.1 245.9 515.1 266.1 502.6 278.6z">
                </path>
            </svg>
        </div>

        <div class="button btn-prev">
            <svg class="svg-inline--fa fa-arrow-left-long" aria-hidden="true" focusable="false" data-prefix="fas"
                data-icon="arrow-left-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                data-fa-i2svg="">
                <path fill="currentColor"
                    d="M9.375 233.4l128-128c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L109.3 224H480c17.69 0 32 14.31 32 32s-14.31 32-32 32H109.3l73.38 73.38c12.5 12.5 12.5 32.75 0 45.25c-12.49 12.49-32.74 12.51-45.25 0l-128-128C-3.125 266.1-3.125 245.9 9.375 233.4z">
                </path>
            </svg>
        </div>
    </div>
</template>

<style scoped>
.button {
    position: absolute;
    z-index: 1;
    top: -70px;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.btn-next {
    cursor: pointer;
    background-color: #00AC4D;
    right: 0;
}

.btn-prev {
    cursor: pointer;
    background-color: white;
    color: black;
    right: 50px;
}

.button>svg {
    width: 40%;
}

.title {
    font-size: 18px;
    font-weight: 600;
    margin-bottom: 6px;
}

.text {
    font-size: 14px;
}

.carousel-card {
    width: 313px;
}

.img-container {
    width: 100%;
    margin-bottom: 18px;
}
</style>