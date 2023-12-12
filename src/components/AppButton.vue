<script>
export default {
    name: 'AppButton',
    props: {
        playBtn: Boolean,
        btnArrow: Boolean,
        text: String
    }
}
</script>

<template>
    <div class="d-flex">
        <button class="button d-flex align-items-center justify-content-center me-3">
            <span class="me-2">{{ text }}</span>
            <svg v-if="btnArrow" class="svg-inline--fa fa-right-long" aria-hidden="true" focusable="false" data-prefix="fas"
                data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg="">
                <path fill="currentColor"
                    d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z">
                </path>
            </svg>
        </button>

        <button v-if="playBtn" class="play-btn">
            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="play"
                role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512" data-fa-i2svg="">
                <path fill="currentColor"
                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                </path>
            </svg>
        </button>
    </div>
</template>

<style scoped>
.play-btn {
    background-color: #05CC7C;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    border: 2px solid #05CC7C;
    display: flex;
    justify-content: center;
    align-items: center;
}

.play-btn>svg {
    width: 18px;
}

.button {
    background-color: #05CC7C;
    border: 2px solid #05CC7C;
    padding: 12px 30px;
    border-radius: 8px;
    font-size: 18px;
    font-weight: 600;
    transition: all 0.3s ease;
}

.button:hover {
    background-color: transparent;
    color: #05CC7C;
}

.button>svg {
    width: 18px;
}
</style>