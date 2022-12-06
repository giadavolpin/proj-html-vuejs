<template>
    <nav>
        <div class="d-flex ">
            <div class="align-content-end">
                <img class="allin" src="/image/takeout-logo.png" alt="">
            </div>
            <div class="d-flex"> 
                <ul>
                    <li v-for="(item,index) in navbar" :key="index">{{item.name}}</li>
                </ul>
                <i class="fa-solid fa-cart-shopping bianco allineamento"></i>           
            </div>
        </div>

        <div>
            <div class="pallinorosso">
                <span class="d-flex justify-content-center piu">+</span>
            </div>
        </div>
    </nav>
    <Jumbotron cognome="Volpin"/>
</template>

<script>
import Jumbotron from './Jumbotron.vue';

export default {
    name: 'HeaderComponent',
    components: {
        Jumbotron
    },
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
li:hover {
    color: $giallo; 
}
.allin{
    padding-top: 40px;
    padding-left: 100px;

}
.allineamento{
    padding-top: 65px;
    padding-left: 15px;
    cursor: pointer;
}
i:hover{
    color: $giallo;
}
ul {
    color: $white;
    list-style-type: none;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    cursor: pointer;
    padding-top: 60px;
    padding-left: 300px;    
}
li{
    padding-left: 30px;
}
.bianco {
    color: white;
}

nav {
    background-color: rgb(25, 6, 7);
    height: 100px;
    position: relative;
}

.pallinorosso {
    height: 50px;
    width: 50px;
    border-radius: 50%;
    background-color: $rosso;
    color: white;
    position: absolute;
    bottom: 50px;
    right: 0;
    top: 0px;

    /* sistemare qui */
}
.piu{
    transform: translate(-50%,-50%);
    top: 50%;
    left: 50%;
    position: absolute;
    font-size: 18px;
}
</style>