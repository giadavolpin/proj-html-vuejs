<template>
   <div class="imgback bianco">
        <div class="d-flex justify-content-around">
            <ul class="pt-2 ">
                <li class="text-uppercase"><strong> order online </strong></li>
                 <li v-for="(item,index) in order" :key="index">{{item.name}}</li>
            </ul>
               
            <ul class="pt-2 ">
                <li class="text-uppercase"><strong> navigate</strong></li>
                <li>Home</li>
                <li>Alternate Home</li>
                <li>Menu</li>
                <li>About</li>
                <li>News</li>
                <li>Contact Us</li>
                <li>Cart</li>
            </ul>
      
            <div class="pt-2">    
                <ul class=" ">
                    <li class="text-uppercase"><strong> information</strong></li>
                    <li>My Account</li>
                    <li>Terms Of Service</li>
                    <li>Privacy Policy</li>
                </ul>
                <div class="pt-2">
                    <img class="bordo" src="/public/image/app-store-badge.png" alt="">
                </div>
                <div>    
                    <img class="bordo" src="/public/image/play-store-badge.png" alt="">
                </div>
            </div>

            <ul  class="pt-2">
                <li class="text-uppercase"><strong> opening hours </strong></li>
                <li>Mon - <span class="giallo">10AM to 11PM</span></li>
                <li>Tue- <span class="giallo">10AM to 11PM</span></li>
                <li>Wed - <span class="giallo">10AM to 11PM</span></li>
                <li>Thur -<span class="giallo">10AM to 11PM</span></li>
                <li>Fri - <span class="giallo">10AM to 11PM</span></li>
                <li>Sat - <span class="giallo">10AM to 11PM</span></li>
                <li>Sun - <span class="giallo">10AM to 11PM</span></li>
            </ul>
            <div  class="pt-2">
                <ul>
                    <li class="text-uppercase"><strong> voucher</strong></li>
                    <img class="sconto" src="/public/image/footer-coupon.png" alt="">
                    <li class="bianco ext"> <strong> Just Use The Code</strong></li>
                    <li class="text-uppercase ext giallo"><strong> firstorder</strong></li>
                    <li class="bianco ext"><strong> AtCheckout</strong></li>
                </ul>
            </div>
        </div>  
        
        <div class="">
            <div class="allgv">
                <img  src="/public/image/takeout-logo.png" alt="">
            </div>
            <h2 class="allgv">Stay in The Loop</h2>
            <p class="allgv">Sign up to receive up to date news and offers directly in your inbox:</p>
            <div class="allgv">
                <input class="radius" type="text" placeholder="you@email.com">
            </div>
            <div class="allgv">
                <button type="button" class="btn btn-danger radius text-uppercase">subscribe</button>
            </div>
        </div>

   </div> 
</template>

<script>

export default {
    name: 'FooterComponent',
    data() {
        return{
            order:[
                {
                    name: "Appetizers", 
                    link: "" 
                },
                {
                    name: "Burgers", 
                    link: ""
                },
                {
                    name: "Pizza", 
                    link: ""
                },
                {
                    name: "Fries", 
                    link: ""
                },
                {
                    name: "Sides", 
                    link: ""
                },
                {
                    name: "Desserts", 
                    link: ""
                },
                {
                    name: "Beverages", 
                    link: ""
                },
                {
                    name: "Specials", 
                    link: ""
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/variables' as*;
.imgback{
    background-image: url(public/image/footer-background-scaled.jpg);
    height: 800px;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
.radius{
    border-radius: 20px;
    width: 500px;
}
.allgv{
    margin-top: 20px;
    display: flex;
    justify-content: center;

}
.ext{
    font-size: 12px;
    text-align: center;
}
.giallo{
    color: $giallo;
}
.bianco{
    color: $white;
    
}
li{
    list-style-type: none;
    cursor: pointer;
}
li:hover{
    color: $giallo;
}
.bordo{
    width: 150px;
    cursor: pointer;
    border: 2px solid $white;
    border-radius: 10px;
    margin-bottom: 10px;
}
.sconto{
    width: 100px;
    height: 100px;
}

</style>