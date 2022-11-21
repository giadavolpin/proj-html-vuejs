<template>
    <div class="container">
        <!-- container allineare al centro -->
        <div class="d-flex flex-row justify-content-between">
            <!-- uppercase -->
            <!-- va in centro??  -->
            <div class="">
                <!-- icona -->
                24/7 delivery
            </div>
            <div class="">
                <!-- icona -->
                over 100 dishes
            </div>
            <div class="">
                <!-- icona -->
                in app ordering
            </div>
            <div class="">
                <!-- icona -->
                fast delivery
            </div>
        </div>
        <!--  <h3>Our Most Popular Dishes</h3>
        <div class="cards">
            <div class="card">
                <img src="../image/skin-on-fries-200x286.jpg" alt="">
            </div>
            <div class="card"></div>
            <div class="card"></div>
        </div> -->

    </div>
</template>

<script>
import general from '../assets/general.scss';
import variables from '../assets/variables.scss';
export default {
    name: 'MainComponent',
    general,
    variables,
}
</script>

<style lang="scss" scoped>
.container {
    max-width: 700px;
    height: 700px;
    background-color: white;
    /* gestire con il juntotron alzare di 10cm non usare position */
}
</style>