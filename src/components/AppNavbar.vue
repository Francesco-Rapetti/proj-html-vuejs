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
            <div id="collapse-button" class="d-flex flex-column justify-content-between" @click="collapse()">
                <span class="bar" :class="{ 'top': collapsed }"></span>
                <span class="bar" :class="{ 'mid': collapsed }"></span>
                <span class="bar" :class="{ 'bot': collapsed }"></span>
            </div>
        </div>
    </nav>
</template>

<style scoped>
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
    transition: all 0.5s ease-in-out;
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