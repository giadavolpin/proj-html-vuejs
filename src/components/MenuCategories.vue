<template>
    <div>
    <!-- titolo -->
    <div class="container gvcont d-flex justify-content-around">
        <h4><strong>Menu Categories</strong></h4>
        <button type="button" class="btn btn-danger btngv text-uppercase">view the full menu <i class="fas fa-arrow-circle-right"></i></button>
    </div>
    <!-- cards -->
    <div class="card">
        <img src="" alt="">
    </div>
    
    </div>
</template>

<script>
    export default {
     name:'MenuCategories',   
    }
</script>

<style lang="scss" scoped>
@use '../assets/variables' as *;
.btngv{
    border-radius: 30px;
}
.gvcont{
    margin: 30px;
}

</style>