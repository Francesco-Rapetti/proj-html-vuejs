<script>
export default {
    name: 'AppNavbar',
    data() {
        return {
            collapsed: false
        }
    },

    methods: {
        collapse() {
            this.collapsed = !this.collapsed
        }
    }
}
</script>

<template>
    <nav class="navbar navbar-expand-lg bg-light bg-transparent">
        <div class="container d-flex justify-content-between">
            <a class="navbar-brand" href="#">
                <div id="logo-container">
                    <img class="w-100" src="../assets/img/menulogo.png" alt="">
                </div>
            </a>

            <div class="d-flex gap-4">
                <div class="item d-flex align-items-center">
                    <a href="#">HOME</a>
                    <svg class="svg-inline--fa fa-angle-down" aria-hidden="true" focusable="false" data-prefix="fas"
                        data-icon="angle-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                        data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M192 384c-8.188 0-16.38-3.125-22.62-9.375l-160-160c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L192 306.8l137.4-137.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-160 160C208.4 380.9 200.2 384 192 384z">
                        </path>
                    </svg>
                </div>

                <div class="item d-flex align-items-center">
                    <a href="#">PAGES</a>
                    <svg class="svg-inline--fa fa-angle-down" aria-hidden="true" focusable="false" data-prefix="fas"
                        data-icon="angle-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                        data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M192 384c-8.188 0-16.38-3.125-22.62-9.375l-160-160c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L192 306.8l137.4-137.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-160 160C208.4 380.9 200.2 384 192 384z">
                        </path>
                    </svg>
                </div>

                <div class="item">
                    <a href="#">TOURNAMENT</a>
                </div>

                <div class="item d-flex align-items-center">
                    <a href="#">SHOP</a>
                    <svg class="svg-inline--fa fa-angle-down" aria-hidden="true" focusable="false" data-prefix="fas"
                        data-icon="angle-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                        data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M192 384c-8.188 0-16.38-3.125-22.62-9.375l-160-160c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L192 306.8l137.4-137.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-160 160C208.4 380.9 200.2 384 192 384z">
                        </path>
                    </svg>
                </div>

                <div class="item d-flex align-items-center">
                    <a href="#">BLOG</a>
                    <svg class="svg-inline--fa fa-angle-down" aria-hidden="true" focusable="false" data-prefix="fas"
                        data-icon="angle-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                        data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M192 384c-8.188 0-16.38-3.125-22.62-9.375l-160-160c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L192 306.8l137.4-137.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-160 160C208.4 380.9 200.2 384 192 384z">
                        </path>
                    </svg>
                </div>

                <div class="item">
                    <a href="#">CONTACT</a>
                </div>
            </div>

            <div class="d-flex gap-3">
                <div class="button-container d-flex align-items-center">
                    <svg class="svg-inline--fa fa-magnifying-glass menu-button" aria-hidden="true" focusable="false"
                        data-prefix="fas" data-icon="magnifying-glass" role="img" xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 512 512" data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M500.3 443.7l-119.7-119.7c27.22-40.41 40.65-90.9 33.46-144.7C401.8 87.79 326.8 13.32 235.2 1.723C99.01-15.51-15.51 99.01 1.724 235.2c11.6 91.64 86.08 166.7 177.6 178.9c53.8 7.189 104.3-6.236 144.7-33.46l119.7 119.7c15.62 15.62 40.95 15.62 56.57 0C515.9 484.7 515.9 459.3 500.3 443.7zM79.1 208c0-70.58 57.42-128 128-128s128 57.42 128 128c0 70.58-57.42 128-128 128S79.1 278.6 79.1 208z">
                        </path>
                    </svg>
                </div>

                <div class="button-container d-flex align-items-center position-relative">
                    <span id="chart-counter">0</span>
                    <svg class="svg-inline--fa fa-bag-shopping menu-button" aria-hidden="true" focusable="false"
                        data-prefix="fas" data-icon="bag-shopping" role="img" xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 448 512" data-fa-i2svg="">
                        <path fill="currentColor"
                            d="M112 112C112 50.14 162.1 0 224 0C285.9 0 336 50.14 336 112V160H400C426.5 160 448 181.5 448 208V416C448 469 405 512 352 512H96C42.98 512 0 469 0 416V208C0 181.5 21.49 160 48 160H112V112zM160 160H288V112C288 76.65 259.3 48 224 48C188.7 48 160 76.65 160 112V160zM136 256C149.3 256 160 245.3 160 232C160 218.7 149.3 208 136 208C122.7 208 112 218.7 112 232C112 245.3 122.7 256 136 256zM312 208C298.7 208 288 218.7 288 232C288 245.3 298.7 256 312 256C325.3 256 336 245.3 336 232C336 218.7 325.3 208 312 208z">
                        </path>
                    </svg>
                </div>
            </div>

            <div id="collapse-button" class="d-flex d-md-none flex-column justify-content-between" @click="collapse()">
                <span class="bar" :class="{ 'top': collapsed }"></span>
                <span class="bar" :class="{ 'mid': collapsed }"></span>
                <span class="bar" :class="{ 'bot': collapsed }"></span>
            </div>
        </div>
    </nav>
</template>

<style scoped>
#chart-counter {
    position: absolute;
    background-color: #4350FF;
    width: 30px;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    top: -15px;
    right: -15px;
}

.button-container {
    cursor: pointer;
    background-color: white;
    padding: 14px;
    border-radius: 50%;
}

.menu-button {
    cursor: pointer;
    width: 16px;
    height: 16px;
    color: #333287;
}

a {
    text-decoration: none;
    color: white;
    font-weight: 600;
    font-size: 16px;
}

.item:hover>* {
    color: #00Ac4D;
}

.fa-angle-down {
    width: 16px;
    height: 16px;
}

#logo-container {
    width: 190px;
}

#collapse-button {
    width: 25px;
    height: 20px;
    cursor: pointer;
}

.bar {
    position: relative;
    background-color: white;
    width: 100%;
    height: 3px;
    transition: all 0.3s ease-in-out;
    top: 0;
}

.bar.top {
    transform: rotate(45deg);
    top: 8px;
}

.bar.mid {
    opacity: 0;
}

.bar.bot {
    transform: rotate(-45deg);
    top: -8px;
}
</style>