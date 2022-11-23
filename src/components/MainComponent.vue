<template>
    <!-- OUR MOST POPULAR DISHES -->
    <div class="gvcontainer">
        <div class="">  <!-- top -30px -->
            <div class="d-flex flex-row justify-content-around text-center">
                <div class="text-uppercase">
                    <i class="fa-regular fa-clock"></i>
                    <strong>24/7 delivery</strong>
                </div>
                <div class="text-uppercase">
                    <i class="fa-solid fa-burger"></i>
                    <strong>over 100 dishes </strong>
                </div>
                <div class="text-uppercase">
                    <i class="fa-solid fa-mobile-screen-button"></i>
                    <strong>in app ordering </strong>
                </div>
                <div class="text-uppercase">
                    <i class="fa-solid fa-car"></i>
                    <strong> fast delivery</strong>
                </div>
            </div>
        </div>
        <h2 class="pt-5 text-center"><strong> Our Most Popular Dishes</strong></h2>
        <div class="d-flex flex-row justify-content-center">
            <div class="gvcard">
                <img class="misura" src="public/image/skin-on-fries-400x571.jpg" alt="">
                <h2 class="text-center"><strong> Skin On Fries</strong></h2>
                <h2 class="rosso">$3.00-$6.00</h2>
            </div>
            <div class="gvcard"> 
                <img class="misura" src="public/image/choco-cookie-frappe-400x571.jpg" alt="">
                <h2 class="text-center"><strong> Choco Cookie Frappe</strong></h2>
                <h2 class="rosso">$4.99</h2>
            </div>
            <div class="gvcard"> 
                <img class="misura" src="public/image/donut-burger-400x571.jpg" alt="">
                <h2 class="text-center"><strong>The Donut Burger</strong> </h2>
                <h2 class="rosso">$6.99</h2>
            </div>
        </div>
        <div class="d-flex justify-content-center">
            <button type="button" class="btn btn-danger btngv text-uppercase">Start your order <i class="fas fa-arrow-circle-right"></i></button>
        </div>
    </div>
    <div class="sconto"></div>
<MenuCategories/>

</template>

<script>
import MenuCategories from './MenuCategories.vue';

export default {
    name: 'MainComponent',
   components: { MenuCategories }

 
}
</script>

<style lang="scss" scoped>
@use '../assets/variables' as *;
.container {
    max-width: 700px;
    height: 700px;
    background-color: white;
    /* gestire con il juntotron alzare di 10cm non usare position */
}
.gvcard{
    margin: 10px;
}
.gvcontainer{
    background-color: $white;
    /* margin-top: -30px;
    z-index: 1000; */

}
.btngv{
    border-radius: 30px;
   
}
.rosso{
    color: $rosso;
    font-size: 20px;
    text-align: center;
}
.sconto{
    background-image: url(public/image/sconto.png); 
    height: 360px;
    background-size: cover;
}
.misura{
    width: 350px;
}
</style>