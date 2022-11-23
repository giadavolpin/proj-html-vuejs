<template>
   <div class="imgback bianco">
        <div class="d-flex ">
            <ul class=" ">
                <li class="text-uppercase"><strong> order online </strong></li>
                 <li v-for="(item,index) in order" :key="index">{{item.name}}</li>
            </ul>
               
            <ul class=" ">
                <li class="text-uppercase"><strong> navigate</strong></li>
                <li>Home</li>
                <li>Alternate Home</li>
                <li>Menu</li>
                <li>About</li>
                <li>News</li>
                <li>Contact Us</li>
                <li>Cart</li>
            </ul>
      
            <div class="">    
                <ul class=" ">
                    <li class="text-uppercase"><strong> information</strong></li>
                    <li>My Account</li>
                    <li>Terms Of Service</li>
                    <li>Privacy Policy</li>
                </ul>
                <div class="">
                    <img class="" src="/public/image/app-store-badge.png" alt="">
                </div>
                <div>    
                    <img class="" src="/public/image/play-store-badge.png" alt="">
                </div>
            </div>

            <ul>
                <li class="text-uppercase"><strong> opening hours </strong></li>
                <li>Mon - <span class="giallo">10AM to 11PM</span></li>
                <li>Tue- <span class="giallo">10AM to 11PM</span></li>
                <li>Wed - <span class="giallo">10AM to 11PM</span></li>
                <li>Thur -<span class="giallo">10AM to 11PM</span></li>
                <li>Fri - <span class="giallo">10AM to 11PM</span></li>
                <li>Sat - <span class="giallo">10AM to 11PM</span></li>
                <li>Sun - <span class="giallo">10AM to 11PM</span></li>
            </ul>
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
img{
    width: 150px;
    cursor: pointer;
}
</style>