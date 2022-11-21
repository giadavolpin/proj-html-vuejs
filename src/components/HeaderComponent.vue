<template>
    <nav>
        <div class="d-flex justify-content-around">
            <div class="d-flex">
                <img class="" src="public\image\image\takeout-logo.png" alt="">
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
        <div class="d-flex justify-content-end">
            <div class="d-flex pallinorosso justify-content-center align-items-center">
                <p class="d-flex">+</p>
            </div>
        </div>
    </nav>
</template>

<script>
import general from '../assets/general.scss';
import variables from '../assets/variables.scss';
name: 'HeaderComponent';
export default {
    general,
    variables
}
</script>

<style lang="scss" scoped>
.attivo {
    color: rgb(249, 210, 47);

}

.bianco {
    color: white;
}

nav {
    background-color: black;
}

.pallinorosso {
    height: 33px;
    width: 33px;
    border-radius: 50%;
    background-color: rgb(207, 25, 37);
    color: white;

}
</style>