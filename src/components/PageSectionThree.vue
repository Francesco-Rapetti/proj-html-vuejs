<script>
import AppCarouselOne from './AppCarouselOne.vue'
export default {
    name: 'PageSectionThree',

    components: {
        AppCarouselOne
    },

    methods: {
    },

    mounted() {
    }
}
</script>

<template>
    <div class="wrapper d-flex align-items-center justify-content-center">
        <div class="filter"></div>
        <div class="container position-relative z-index-1">
            <div class="row">
                <div class="col-6 my-auto">
                    <div class="live-thumb position-relative">
                        <img class="w-100" src="../assets/img/v-1.png" alt="live-thumb">

                        <div class="video-area d-flex flex-column justify-content-center align-items-center gap-3">
                            <button class="play-btn position-relative">
                                <div id="btn-animation"></div>
                                <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                    data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                    data-fa-i2svg="">
                                    <path fill="currentColor"
                                        d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                    </path>
                                </svg>
                            </button>

                            <span class="fw-bold">Call Of Deauty</span>
                        </div>
                    </div>
                </div>

                <div class="col-6">
                    <p class="highlight">Live Streaming</p>
                    <h1 class="title">Checkout Our Live Streaming</h1>
                    <AppCarouselOne type="1" :slidesPerView="2" />
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.video-area {
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
}

#btn-animation {
    position: absolute;
    width: 70px;
    height: 70px;
    border-radius: 50%;
    border: 10px solid #00AC4D;
    opacity: 0;
    animation: pulse 1.5s infinite;
    transform: scale(1.75);
}

@keyframes pulse {
    0% {
        transform: scale(1);
        opacity: 1;
        box-shadow: 0 0 0 0 rgba(0, 172, 77, 0.7);
    }
}

.play-btn {
    background-color: #00AC4D;
    width: 70px;
    height: 70px;
    border-radius: 50%;
    border: 2px solid #00AC4D;
    display: flex;
    justify-content: center;
    align-items: center;
}

.play-btn>svg {
    width: 14px;
    color: white;
}

.filter {
    position: absolute;
    width: inherit;
    height: inherit;
    background-color: #0000007b;
}

.wrapper {
    width: 100%;
    height: 750px;
    background-image: url('../assets/img/v-bg.png');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>