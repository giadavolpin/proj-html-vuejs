<template>
    <nav>
        <div class="d-flex justify-content-around">
            <div class="d-flex">
                <img class="" src="../image/takeout-logo.png" alt="">
            </div>
            <div class="d-flex">
                <button type="button" class=" btn attivo dropdown-toggle">Home</button>
                <button type="button" class=" btn bianco">Order Online</button>
                <button type="button" class=" btn bianco">About</button>
                <button type="button" class=" btn bianco">News</button>
                <button type="button" class=" btn bianco">Contact Us</button>
                <button type="button" class=" btn bianco"><i class="fa-solid fa-cart-shopping "></i></button>
                <!-- sistemare fontewesome -->
            </div>
        </div>
        <div class="">
            <!-- sistemare il position:relative -->
            <div class="pallinorosso">
                <p class="d-flex justify-content-center">+</p>
            </div>
        </div>
    </nav>
    <Jumbotron />
</template>

<script>
import general from '../assets/general.scss';
import variables from '../assets/variables.scss';
import Jumbotron from './Jumbotron.vue';

export default {
    name: 'HeaderComponent',
    general,
    variables,
    components: {
        Jumbotron
    },
}
</script>

<style lang="scss" scoped>
.attivo {
    color: rgb(249, 210, 47); //sistemare qui
}

.bianco {
    color: white;
}

nav {
    background-color: rgb(25, 6, 7);
    height: 80px;
    position: relative;
}

.pallinorosso {
    height: 35px;
    width: 35px;
    border-radius: 50%;
    background-color: rgb(207, 25, 37);
    color: white;
    position: absolute;
    /* sistemare qui */
}
</style>