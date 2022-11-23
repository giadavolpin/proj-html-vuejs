<template>
    <div>
    <!-- titolo -->
        <div class="container gvcont">
            <h2 class="pl"><strong>Menu Categories</strong></h2>
            <button type="button" class="btn btn-danger btngv text-uppercase">view the full menu  <i class="p-1 fas fa-arrow-circle-right"></i></button>
        </div>
        <!-- cards menu-->
        <div class="d-flex row container center">
            <div class="flex-wrap col-3" v-for="(item,index) in menu" :key="index">
                <img class="imggv" :src="item.img" alt="">    
            </div>
        </div>
        <div class="container d-flex flex-row justify-content-around mt-3 mb-2">
            <div class="flex">
                <img src="/public/image/vegetarian.png" alt="">
                <p class="p-1">Vegetarian</p>
            </div>
            <div class="flex">
                <img src="/public/image/grano.png" alt="">
                <p class="p-1">Gluten Free</p>
            </div>
            <div class="flex">
                <img src="/public/image/latte.png" alt="">
                <p class="p-2">Dairy Free</p>
            </div>
            <div class="flex">
                <img src="/public/image/keto.png" alt="">
                <p class="p-1">Keto Friendly</p>
            </div>
        </div>
    </div>
    <div class="orderapp">
        <div class="container d-flex flex-column justify-content-center">
            <h4 class="bianco mt-5">Download Our</h4>
            <h1 class="giallo mb-2">Ordering App</h1>
        </div>
        <div class="d-flex row centro">
            <img class="imgstore" src="/public/image/app-store-badge.png" alt="">
            <img class="imgstore" src="/public/image/play-store-badge.png" alt="">
        </div>
    </div>
    <!-- LATEST NEWS -->
    <div class="container d-flex gvcont">
        <h2 class="pl"><strong>Latest News</strong></h2>
        <button type="button" class="btn btn-danger btngv text-uppercase">read more news<i class="p-1 fas fa-arrow-circle-right"></i></button>
    </div>
    <div class="container d-flex flex-row">
        <div class="text-center ">
            <img class="prgv imgmis" src="/public/image/pancake-burger-600x450.jpg" alt="">
            <h3 class="prgv p-2"><strong>NEW: The Pancake Burger</strong></h3>
            <p class="picc prgv">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente repellat eius culpa quo ut nisi debitis dolorum nam, rerum eum! Ratione inventore recusandae sed impedit iusto hic fuga reprehenderit laboriosam.</p>
        </div>
        <div class="text-center">
            <img class="imgmis" src="/public/image/new-milkshake-menu-600x450.jpg" alt="">
            <h3 class="p-2"><strong>New Milkshake Menu</strong></h3>
            <p class="piccolo">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente repellat eius culpa quo ut nisi debitis dolorum nam, rerum eum! Ratione inventore recusandae sed impedit iusto hic fuga reprehenderit laboriosam.</p>
        </div>
    </div>
</template>

<script>
    export default {
     name:'MenuCategories',   
     
     data() {
            return {
               menu: [
            {
                id: '1',
                img: '/public/image/appetizers-menu-background.jpg'
            },
            {
                id: '2',
                img: '/public/image/burgers-menu-background.jpg'
            },
            {
                id: '3',
                img: '/public/image/pizza-menu-background.jpg'
            },
            {
                id: '4',
                img: '/public/image/fries-menu-background.jpg'
            },
            {
                id: '5',
                img: '/public/image/sides-menu-background.jpg'
            },
            {
                id: '6',
                img: '/public/image/desserts-menu-background.jpg'
            },
            {
                id: '7',
                img: '/public/image/beverages-menu-background.jpg'
            },
            {
                id: '8',
                img: '/public/image/specials-menu-background.jpg'
            }
            ]
    }}
    }
</script>

<style lang="scss" scoped>
@use '../assets/variables' as *;
.btngv{
    border-radius: 30px;
    display: flex;
    align-items: center;
    flex-direction: flex-end;
}
.gvcont{
    margin: 30px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 50px;
    margin-top: 70px;
}
.giallo{
    color: $giallo;
    font-size: 48px;
}
.bianco{
    color: $white;
    margin-bottom: 0;
}
.center{
    margin-left: 100px;
}
.orderapp{
    background-image: url(public/image/app-ordering-scaled.jpg);
    height: 350px;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
.imggv{
    width: 100%;
    padding-bottom: 20px;
}
.gvcontainer{
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    flex-wrap: wrap;
}
.imgstore{
    width: 130px;
    margin: 10px;
    margin-top: 20px;
    
}
.centro{
    margin-left: 100px;
}
.pl{
    padding-left: 80px;
}
.piccolo{
    font-size: 14px;
    margin-left: 50px;
    margin-right: 50px;
}
.picc{
    font-size: 14px;
}
.prgv{
    margin-right: 20px;
}
.imgmis{
    width: 535px;
    height: 430px;
}
</style>