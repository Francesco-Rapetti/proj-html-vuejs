<script>
import AppButton from './AppButton.vue'
export default {
    name: 'PageSectionOne',
    components: {
        AppButton
    },

    data() {
        return {

        }
    },

    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="d-flex justify-content-center align-items-center">
            <div>
                <div class="img-container position-relative">
                    <img id="raiden" class="w-100" :src="getImagePath('exprince.jpg')" alt="">
                    <img id="shape1" :src="getImagePath('shape1.png')" alt="">
                    <img id="shape2" :src="getImagePath('shape2.png')" alt="">
                    <img id="shape3" :src="getImagePath('exprience-shape.png')" alt="">
                </div>
            </div>

            <div class="m-5">
                <p id="subtitle">12 Year Experience</p>
                <h1>We Are The Best Gaming Company</h1>
                <p class="mb-3">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim autem asperiores facere ab,
                    officia,
                    provident, placeat non quas recusandae alias debitis. Assumenda non quos, tempora optio excepturi
                    accusamus facilis in.</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa est ex beatae voluptatum distinctio. Velit,
                    aliquid</p>
                <div class="d-flex align-items-center mt-4">
                    <div class="icon me-3">
                        <svg class="svg-inline--fa fa-check" aria-hidden="true" focusable="false" data-prefix="fas"
                            data-icon="check" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M438.6 105.4C451.1 117.9 451.1 138.1 438.6 150.6L182.6 406.6C170.1 419.1 149.9 419.1 137.4 406.6L9.372 278.6C-3.124 266.1-3.124 245.9 9.372 233.4C21.87 220.9 42.13 220.9 54.63 233.4L159.1 338.7L393.4 105.4C405.9 92.88 426.1 92.88 438.6 105.4H438.6z">
                            </path>
                        </svg>
                    </div>
                    <p class="list">Sed porttitor lectus nibh. Proin eget tortor risus</p>
                </div>
                <div class="d-flex align-items-center mt-3">
                    <div class="icon me-3">
                        <svg class="svg-inline--fa fa-check" aria-hidden="true" focusable="false" data-prefix="fas"
                            data-icon="check" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M438.6 105.4C451.1 117.9 451.1 138.1 438.6 150.6L182.6 406.6C170.1 419.1 149.9 419.1 137.4 406.6L9.372 278.6C-3.124 266.1-3.124 245.9 9.372 233.4C21.87 220.9 42.13 220.9 54.63 233.4L159.1 338.7L393.4 105.4C405.9 92.88 426.1 92.88 438.6 105.4H438.6z">
                            </path>
                        </svg>
                    </div>
                    <p class="list">Praesent sapien massa, convallis a pellentesque nec. risus.</p>
                </div>
                <div class="d-flex align-items-center mt-3">
                    <div class="icon me-3">
                        <svg class="svg-inline--fa fa-check" aria-hidden="true" focusable="false" data-prefix="fas"
                            data-icon="check" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M438.6 105.4C451.1 117.9 451.1 138.1 438.6 150.6L182.6 406.6C170.1 419.1 149.9 419.1 137.4 406.6L9.372 278.6C-3.124 266.1-3.124 245.9 9.372 233.4C21.87 220.9 42.13 220.9 54.63 233.4L159.1 338.7L393.4 105.4C405.9 92.88 426.1 92.88 438.6 105.4H438.6z">
                            </path>
                        </svg>
                    </div>
                    <p class="list">Praesent sapien massa, convallis a pellentesque nec. risus.</p>
                </div>
                <div class="d-flex align-items-center mt-3">
                    <div class="icon me-3">
                        <svg class="svg-inline--fa fa-check" aria-hidden="true" focusable="false" data-prefix="fas"
                            data-icon="check" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M438.6 105.4C451.1 117.9 451.1 138.1 438.6 150.6L182.6 406.6C170.1 419.1 149.9 419.1 137.4 406.6L9.372 278.6C-3.124 266.1-3.124 245.9 9.372 233.4C21.87 220.9 42.13 220.9 54.63 233.4L159.1 338.7L393.4 105.4C405.9 92.88 426.1 92.88 438.6 105.4H438.6z">
                            </path>
                        </svg>
                    </div>
                    <p class="list">Praesent sapien massa, convallis a pellentesque nec. risus.</p>
                </div>


                <div class="mt-5">
                    <AppButton text="Discover More" :btnArrow="true" :playBtn="true" />
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    margin-bottom: 6rem;
}

#subtitle {
    color: #00AC4D;
    font-weight: 600;
    font-size: 18px;
}

.list {
    font-weight: 600;
}

h1 {
    font-size: 50px;
    font-weight: 700;
    margin: 1rem 0 2rem 0;
}

.icon {
    width: 24px;
    height: 24px;
    color: #00AC4D;
    border: 1px solid #00AC4D;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.icon>svg {
    width: 60%;
    height: 60%;
}

.img-container {
    width: 484px;
    height: 484px;
    margin: 100px;
}

#shape1 {
    position: absolute;
    top: -50px;
    left: -50px;
    z-index: -1;
    width: 450px;
}

#shape2 {
    position: absolute;
    z-index: -1;
    bottom: -30px;
    right: -30px;
}

#shape3 {
    position: absolute;
    z-index: -1;
    top: -20px;
    left: -130px;
}
</style>