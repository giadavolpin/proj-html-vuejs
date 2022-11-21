<template>
    <!-- JUMBOTRON -->
    <div class="jumbotron d-flex ">
        <div class="row justify-content-center align-content-center">
            <h3 class="bianco col-7">Hungry?</h3>
            <h1 class=" giallo col-7">Great Food</h1>
            <h1 class="bianco col-7">Delivered</h1>

        </div>
        <div>
            <!-- bottone a lato -->
        </div>
        <div>
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
    color: rgb(249, 210, 47);
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
</style>