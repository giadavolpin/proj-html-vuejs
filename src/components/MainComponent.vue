<template>
    <div class="container gvcontainer">
        <!-- container allineare al centro -->
        <div class="d-flex flex-row justify-content-between">
            <!-- va in centro??  -->
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
        <h3 class="pt-5 text-center">Our Most Popular Dishes</h3>
        <div class="d-flex flex-row">
            <div class="gvcard">
                <img src="public/image/skin-on-fries-200x286.jpg" alt="">
                <p class="text-center"><strong> Skin On Fries</strong></p>
                <p class="rosso">$3.00-$6.00</p>
            </div>
            <div class="gvcard"> 
                <img src="public/image/choco-cookie-frappe-200x286.jpg" alt="">
                <p class="text-center"><strong> Choco Cookie Frappe</strong></p>
                <p class="rosso">$4.99</p>
            </div>
            <div class="gvcard"> 
                <img src="public/image/donut-burger-200x286.jpg" alt="">
                <p class="text-center"><strong>The Donut Burger</strong> </p>
                <p class="rosso">$6.99</p>
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
    font-size: 10px;
    text-align: center;
}
.sconto{
    background-image: url(public/image/sconto.png); 
    height: 360px;
    background-size: cover;
}
</style>