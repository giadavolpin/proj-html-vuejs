<template>
    <!-- JUMBOTRON -->
    <div class="jumbotron">
        <div class="d-flex flex-column">
            <h3 class="bianco">Hungry?</h3>
            <h1 class=" giallo">Great Food</h1>
            <h1 class="bianco">Delivered</h1>
        </div>
        <div class="">
            <div class="rosso">
                <p class=""> view our menu</p>
                <div class="">
                    <!-- icona  -->
                </div>
            </div>
        </div>
        <div class="btnbianco">
            <!-- bottone a lato -->
        </div>
        <div class="btnbianco">
            <!-- bottone a lato -->
        </div>
    </div>
</template>

<script>
import general from '../assets/general.scss';
import variables from '../assets/variables.scss';

export default {
    name: 'Jumbotron',
    general,
    variables,

}
</script>

<style lang="scss" scoped>
.giallo {
    color: rgb(252, 214, 108);
}

.bianco {
    color: white;
}

.jumbotron {
    height: 560px;
    background-image: url(../image/home-background-hero-scaled.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

}

.rosso {
    background-color: rgb(204, 26, 38);
    color: white;
    border-radius: 30px;
    text-align: center;
}

.btnbianco {
    height: 45px;
    width: 45px;
    background-color: white;
}
</style>