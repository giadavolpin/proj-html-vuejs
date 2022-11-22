<template>
    <nav>
        <div v-bind="props"></div>
        <div class="d-flex justify-content-around" v-for="(item, index) in intestazione, key = id ">
            <img :src="item.img">
            <button>{{ item.text }}</button> -->
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
    data() {
        return {
            props: ['src', 'text', "icona"],
        }
    },
    created: {
        console.log(props),
    }
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
    bottom: 50px;
    right: 0;
    top: -55px;

    /* sistemare qui */
}
</style>