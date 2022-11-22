<template>
    <nav>
        <div class="d-flex justify-content-between">
            <div>
            <img class="" src="/image/takeout-logo.png" alt="">
            </div>
            <div class="d-flex">
                <ul>
                    <li v-for="(item,index) in navbar" :key="index">{{item.name}}</li>
                </ul>
                <!-- icona -->
            
            </div>
        </div>

        <div>
            <!-- sistemare il position:relative -->
            <div class="pallinorosso">
                <p class="d-flex justify-content-center">+</p>
            </div>
        </div>
    </nav>
    <Jumbotron />
</template>

<script>
import Jumbotron from './Jumbotron.vue';

export default {
    name: 'HeaderComponent',
    components: {
        Jumbotron
    },
    props: ['src', 'text', "icona"],
    data() {
        return {
        navbar: [
            {
                name: "Home", 
                link: ""
            },
            {
                name: "Order Online", 
                link: ""
            },
            {
                name: "About", 
                link: ""
            },
            {
                name: "News", 
                link: ""
            },
            {
                name: "Contact Us", 
                link: ""
            },
        ]      
        }
    },
     
}


</script>

<style lang="scss" scoped>
@use '../assets/variables' as*;
.attivo {
    color: rgb(249, 210, 47); //sistemare qui
}
ul {
    color: $white;
    /* sistemare altro */
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
    bottom: 50px;
    right: 0;
    top: -55px;

    /* sistemare qui */
}
</style>