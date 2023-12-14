<script></script>

<template>
    <div class="wrapper position-relative">
        <div class="filter"></div>
        <div class="container top">
            <div class="row">
                <div class="col-6">
                    <h1 id="news-letter-text">Our news Letter</h1>
                </div>

                <div class="col-6">
                    <div class="input-text">
                        <div class="d-flex align-items-center">
                            <div class="icon d-flex align-items-center justify-content-center">
                                <svg class="svg-inline--fa fa-message" aria-hidden="true" focusable="false"
                                    data-prefix="fas" data-icon="message" role="img" xmlns="http://www.w3.org/2000/svg"
                                    viewBox="0 0 512 512" data-fa-i2svg="">
                                    <path fill="currentColor"
                                        d="M511.1 63.1v287.1c0 35.25-28.75 63.1-64 63.1h-144l-124.9 93.68c-7.875 5.75-19.12 .0497-19.12-9.7v-83.98h-96c-35.25 0-64-28.75-64-63.1V63.1c0-35.25 28.75-63.1 64-63.1h384C483.2 0 511.1 28.75 511.1 63.1z">
                                    </path>
                                </svg>
                            </div>
                            <input type="text" name="" id="" placeholder="Enter your email">
                        </div>
                        <button>Subscribe</button>
                    </div>
                </div>
            </div>
        </div>

        <div class="container">

        </div>
    </div>
</template>

<style scoped>
.container {
    z-index: 1;
    position: relative;
}

.filter {
    position: absolute;
    width: inherit;
    height: inherit;
    background-color: #19193578;
}

.wrapper {
    width: 100%;
    height: 374px;
    background-image: url(../assets/img/footer-bg.png);
}

button {
    background-color: #00AC4D;
    color: black;
    border: 0;
    border-radius: 24px;
    padding: 12px 20px;
    font-weight: 600;
}

input {
    background-color: transparent;
    border: 0;
    color: grey;
    padding-left: 1rem;
}

input:focus {
    outline: 0;
}

.input-text {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #191935;
    padding: 10px 15px;
    border-radius: 50px;
}

.icon {
    width: 16px;
    height: 16px;
    color: #00AC4D;
}

#news-letter-text {
    color: white;
    font-size: 36px;
    font-weight: 700;
}

.container.top {
    padding: 60px 40px;
    background-color: #202046;
    border-radius: 8px;
    top: -100px;
}
</style>