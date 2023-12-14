<script>
export default {
    name: 'PageSectionTwo',

    data() {
        return {
            cards: [
                {
                    img: 'feature1.png',
                    title: 'Live Streaming',
                    text: 'Nulla porttutor accusan tincidunt. Pellentesque in.'
                }, {
                    img: 'feature2.png',
                    title: 'Gaming News',
                    text: 'Nulla porttitor accusan tincidunt. Pellentesque in.'
                }, {
                    img: 'feature3.png',
                    title: 'Great Tournament',
                    text: 'Nulla porttitor accusan tincidunt. Pellentesque in.'
                }, {
                    img: 'feature4.png',
                    title: 'Awward Ceremony',
                    text: 'Nulla porttitor accusan tincidunt. Pellentesque in.'
                }
            ]
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
    <div class="wrapper position-relative d-flex align-items-center">
        <div class="filter"></div>
        <div class="container z-index-1 position-relative">
            <div class="row align-items-center">
                <div class="col-6">
                    <div class="me-5">
                        <p class="highlight">Our Extreme Features</p>
                        <h1 class="title">The Best Gaming Arena On The World!</h1>
                        <p class="fs-6">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, in totam harum recusandae
                            consequatur, illo, accusamus ducimus ea iste excepturi neque quisquam nisi ex eos voluptatibus
                            aspernatur vitae. Porro, dolorum.
                        </p>
                    </div>
                </div>

                <div class="col-6">
                    <div class="d-flex flex-wrap gap-4">
                        <div v-for="card in cards" class="feature-card">
                            <div class="feature-img">
                                <img :src="getImagePath(card.img)" :alt="card.img">
                            </div>

                            <h4>{{ card.title }}</h4>
                            <p class="fs-6">{{ card.text }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.feature-img {
    width: 100px;
    height: 100px;
    background-color: #202046;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 20px;
    margin-top: 10px;
}

.feature-img>img {
    max-width: 60px;
    max-height: 60px;
}

.feature-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #333287;
    padding: 40px 30px;
    border-radius: 16px;
    width: 306px;
    height: 317px;
    text-align: center;
    transition: all 0.3s ease;
}

.feature-card * {
    transition: all 0.3s ease;
}

.feature-card:hover {
    background-color: #05CC7C;
    color: black;
}

.feature-card:hover .feature-img {
    transform: scale(1.1);
}

.filter {
    position: absolute;
    width: inherit;
    height: inherit;
    background-color: #2020466d;
}

.wrapper {
    width: 100%;
    height: 900px;
    background-image: url('../assets/img/Vector.png');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>