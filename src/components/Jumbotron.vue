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
        <div class="btnbianco btnsopra">
            <!-- bottone a lato -->
        </div>
        <div class="btnbianco btnsotto">
            <!-- bottone a lato -->
        </div>
    </div>
</template>

<script>
export default {
    name: 'Jumbotron'
}
</script>

<style lang="scss" scoped>
@use '../assets/variables' as *;
.giallo {
    color: $giallo;
}

.bianco {
    color: $white;
}

.jumbotron {
    height: 560px;
    background-image: url(../image/home-background-hero-scaled.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    /* sistemare qui */
}

.rosso {
    background-color: rgb(204, 26, 38);
    color: white;
    border-radius: 20px;
    text-align: center;
    position: absolute;
}

.btnbianco {
    height: 45px;
    width: 45px;
    background-color: white;
    border-radius: 10px;
}

.btnsopra {
    position: absolute;
    right: 10 px;
    top: 10px;
}

.btnsotto {
    position: absolute;
    right: 10px;
    top: 60px;
}
</style>