<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation } from 'swiper/modules';
import { Autoplay } from 'swiper/modules';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/autoplay';

export default {
    components: {
        Swiper,
        SwiperSlide
    },

    data() {
        return {
            autoplay: true
        }
    },

    setup() {
        return {
            modules: [Navigation, Autoplay],
        };
    },
}
</script>

<template>
    <div class="carousel position-relative">
        <Swiper :modules="modules" :slides-per-view="4" :space-between="20" :loop="true" :autoplay="{
            autoplay: true,
            pauseOnMouseEnter: true,
        }" :navigation="{ nextEl: '.btn-next', prevEl: '.btn-prev' }">
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio1.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio2.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio3.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio4.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card position-relative">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio1.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio2.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio3.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <span class="new">New</span>
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/protfolio4.png" alt="">
                    </div>
                    <div id="main-content" class="d-flex align-items-center justify-content-between">
                        <div class="w-75">
                            <p class="title">Assassin's creed</p>
                            <p class="text">Donec sollicitudin malesuada</p>
                        </div>
                        <div class="play-btn">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg>
                        </div>
                    </div>
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
.new {
    position: absolute;
    top: 0;
    left: 0;
    background-color: #05CC7C;
    color: black;
    padding: 4px 13px;
}

#main-content {
    padding: 20px 15px;
}

.play-btn {
    background-color: #05CC7C;
    color: black;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
}

.play-btn>svg {
    width: 15px;
}

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
    background-color: #202046;
    width: 300px;
    transition: all 0.3s ease;
}

.carousel-card:hover {
    background-color: #05CC7C;
    color: black;
}

.carousel-card:hover .play-btn {
    background-color: black !important;
    color: #05CC7C !important;
}

.img-container {
    width: 100%;
}
</style>