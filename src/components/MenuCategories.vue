<template>
    <div>
    <!-- titolo -->
        <div class="container gvcont">
            <h2><strong>Menu Categories</strong></h2>
            <button type="button" class="btn btn-danger btngv text-uppercase">view the full menu <i class="fas fa-arrow-circle-right"></i></button>
        </div>
        <!-- cards -->
        <div class="d-flex container" v-for="(item,index) in menu" :key="index">
             {{item.img}}   
        </div>
        <div class="container d-flex flex-row justify-content-around">
            <div>
                <img src="/public/image/vegetarian.png" alt="">
                <p class="p-1">Vegetarian</p>
            </div>
            <div>
                <img src="/public/image/grano.png" alt="">
                <p class="p-1">Gluten Free</p>
            </div>
            <div>
                <img src="/public/image/latte.png" alt="">
                <p class="p-2">Dairy Free</p>
            </div>
            <div>
                <img src="/public/image/keto.png" alt="">
                <p class="p-1">Keto Friendly</p>
            </div>
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
                img: '/public/image/first-order-background-scaled.jpg'
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
}

</style>