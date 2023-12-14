<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation } from 'swiper/modules';
import AppButton from './AppButton.vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';

export default {
    components: {
        Swiper,
        SwiperSlide,
        AppButton
    },

    data() {
        return {
        }
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
        <Swiper :modules="modules" :slides-per-view="4" :space-between="20" :loop="true"
            :navigation="{ nextEl: '.btn-next', prevEl: '.btn-prev' }">
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b1.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Ninja Warrior Gaming</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b2.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Ghost Rider Returns</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b3.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Call Of Duty 4</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b4.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Mortal Kombat X</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>
            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b1.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Ninja Warrior Gaming</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b2.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Ghost Rider Returns</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b3.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Call Of Duty 4</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
                        </div>
                    </div>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="carousel-card">
                    <div class="img-container">
                        <img class="w-100" src="../assets/img/b4.png" alt="">
                    </div>
                    <div id="main-content" class="text-center d-flex flex-column justify-content-center align-items-center">
                        <div>
                            <p class="title mb-3">Mortal Kombat X</p>
                            <div class="d-flex mb-4">
                                <div class="youtube d-flex">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-youtube" aria-hidden="true" focusable="false"
                                            data-prefix="fab" data-icon="youtube" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">By Admin</p>
                                </div>

                                <div class="d-flex align-items-center">
                                    <div class="icon">
                                        <svg class="svg-inline--fa fa-calendar-days" aria-hidden="true" focusable="false"
                                            data-prefix="fas" data-icon="calendar-days" role="img"
                                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" data-fa-i2svg="">
                                            <path fill="currentColor"
                                                d="M160 32V64H288V32C288 14.33 302.3 0 320 0C337.7 0 352 14.33 352 32V64H400C426.5 64 448 85.49 448 112V160H0V112C0 85.49 21.49 64 48 64H96V32C96 14.33 110.3 0 128 0C145.7 0 160 14.33 160 32zM0 192H448V464C448 490.5 426.5 512 400 512H48C21.49 512 0 490.5 0 464V192zM64 304C64 312.8 71.16 320 80 320H112C120.8 320 128 312.8 128 304V272C128 263.2 120.8 256 112 256H80C71.16 256 64 263.2 64 272V304zM192 304C192 312.8 199.2 320 208 320H240C248.8 320 256 312.8 256 304V272C256 263.2 248.8 256 240 256H208C199.2 256 192 263.2 192 272V304zM336 256C327.2 256 320 263.2 320 272V304C320 312.8 327.2 320 336 320H368C376.8 320 384 312.8 384 304V272C384 263.2 376.8 256 368 256H336zM64 432C64 440.8 71.16 448 80 448H112C120.8 448 128 440.8 128 432V400C128 391.2 120.8 384 112 384H80C71.16 384 64 391.2 64 400V432zM208 384C199.2 384 192 391.2 192 400V432C192 440.8 199.2 448 208 448H240C248.8 448 256 440.8 256 432V400C256 391.2 248.8 384 240 384H208zM320 432C320 440.8 327.2 448 336 448H368C376.8 448 384 440.8 384 432V400C384 391.2 376.8 384 368 384H336C327.2 384 320 391.2 320 400V432z">
                                            </path>
                                        </svg>
                                    </div>
                                    <p class="ms-2">Oct 25, 2022</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-2 mb-3">
                            <AppButton text="Read More" :btnArrow="true" />
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
.youtube {
    padding-right: 10px;
    margin-right: 10px;
    border-right: 1px solid #00AC4D;
}

.icon {
    width: 18px;
    color: #00AC4D;
}

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
    font-size: 24px;
    font-weight: 700;
    margin-bottom: 6px;
}

.text {
    font-size: 14px;
}

.carousel-card {
    background-color: #202046;
    width: 300px;
    transition: all 0.3s ease;
    border-radius: 16px;
}

* {
    transition: all 0.3s ease;
}

.carousel-card:hover img {
    transform: scale(1.1);
}

.carousel-card:hover .title {
    color: #00AC4D;
}

.img-container {
    width: 100%;
    overflow: hidden;
}
</style>