<script>

export default {
    data() {
        return {
            sponsors: ["../src/assets/client-logo-01.png", "../src/assets/client-logo-02.png", "../src/assets/client-logo-03.png", "../src/assets/client-logo-04.png", "../src/assets/client-logo-05.png", "../src/assets/client-logo-06.png"]
        }
    },
}


</script>
<!-- Copertina iniziale della pagina statica con caricamento degli sponsor con ciclo for su un array -->
<template>
    <div class="container py-5">
        <!-- Creazione della grafica con immagine pricipale e vari elementi di sfondo -->
        <div class="row align-items-center">
            <div class="col-5 d-flex flex-column">
                <h1 class="colorTitles">Distant learning for further expansion</h1>
                <p class="colorText">Learning is a life-long journey that in fact we never find the terminate stop. Stop
                    searching, enjoy the
                    process.</p>
                <span><button type="button" class="btnCustom rounded">Download free guide</button></span>
                <span class="colorText py-3">Have questions? <a href="" class="colorVipText fw-bold greenHov">Get Free
                        Sample
                        &rarr;</a></span>
            </div>
            <div class="col-7 imgBackJumbo text-center rlt">
                <img src="../assets/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt=""
                    class="imgJumbo">
                <span class="cerchio"></span>
            </div>
        </div>
        <div class="row align-items-center mt-5">
            <!-- Ciclo for del caricamento immagini -->
            <template v-for="sponsor in sponsors">
                <div class="col-2">
                    <img :src="sponsor" alt="" class="img-fluid">
                </div>
            </template>
        </div>
    </div>
</template>

<style  lang="scss" scoped>
@use '../styles/variables.scss' as *;

.imgJumbo {
    border-radius: 100%;
    background-image: url(../assets/maxcoach-shape-02.png);
    width: 65%;
}

.imgBackJumbo {
    background-image: url(../assets/maxcoach-shape-02.png), url(../assets/maxcoach-shape-07-100x100.png), url(../assets/maxcoach-shape-08.png), url(../assets/maxcoach-shape-08.png);
    background-position: 100% 20%, 70% 100%, 10% 30%, 10% 70%;
    background-repeat: no-repeat;
}

.rlt {
    position: relative;
}

.cerchio {
    height: 70px;
    width: 70px;
    border: 10px solid #ecc5ab;
    border-radius: 50%;
    position: absolute;
    right: 79%;
    bottom: 22%;
}

.greenHov:hover {
    color: $ColorHover;
}
</style>