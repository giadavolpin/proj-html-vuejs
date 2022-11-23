<template>
    <!-- JUMBOTRON prima schermata -->
    <div class="jumbotron">
        <div class="d-flex flex-column container">
            <h3 class="gvpt bianco">Hungry?</h3>
            <h1 class="giallo">Great Food</h1>
            <h1 class="bianco">Delivered</h1>
        </div>
        <div class="d-flex container">
            <button type="button" class="btn btn-danger btngv text-uppercase">view our menu <i class="fas fa-arrow-circle-right"></i></button>
        </div>
       <!-- btn fissi nella pagina -->
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
.btngv{
    border-radius: 30px;
   
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
    background-color: $rosso;
    color: $white;
    border-radius: 20px;
    position: absolute;
    width: 160px;
    display: flex;
    justify-content: center;
    align-content: center;    //sistemare qui
}

.btnbianco {
    height: 65px;
    width: 65px;
    background-color: white;
    border-radius: 10px;
    overflow: hidden;
    flex-direction: column;
    align-items: center;
    cursor: pointer;
    background-color: $white;
    border-radius: 6px;
}

.btnsopra {
    position: absolute; 
}
.btnsotto {
    position: absolute;
}
.gvpt{
    padding-top: 80px;
}
</style>