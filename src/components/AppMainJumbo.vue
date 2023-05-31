<script>

export default {
    data() {
        return {
            sponsors: ["../src/assets/client-logo-01.png", "../src/assets/client-logo-02.png", "../src/assets/client-logo-03.png", "../src/assets/client-logo-04.png", "../src/assets/client-logo-05.png", "../src/assets/client-logo-06.png"]
        }
    },
}


</script>

<template>
    <div class="container py-5">
        <div class="row align-items-center">
            <div class="col-5 d-flex flex-column">
                <h1 class="colorTitles">Distant learning for further expansion</h1>
                <p>Learning is a life-long journey that in fact we never find the terminate stop. Stop searching, enjoy the
                    process.</p>
                <button type="button" class="btn btn-success">Download free guide</button>
                <span>Have questions? <a href="">Get Free Sample -.-></a></span>
            </div>
            <div class="col-7 imgBackJumbo text-center">
                <img src="../assets/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt=""
                    class="imgJumbo">
            </div>
        </div>
        <div class="row align-items-center mt-5">
            <template v-for="sponsor in sponsors">
                <div class="col-2">
                    <img :src="sponsor" alt="" class="img-fluid">
                </div>
            </template>
        </div>
    </div>
</template>

<style scoped>
.imgJumbo {
    border-radius: 100%;
    background-image: url(../assets/maxcoach-shape-02.png);
    width: 65%;
}

.imgBackJumbo {
    background-image: url(../assets/maxcoach-shape-02.png), url(../assets/maxcoach-shape-07-100x100.png), url(../assets/maxcoach-shape-08.png);
    background-position: 100% 20%, 70% 100%, 10% 50%;
    background-repeat: no-repeat;
}
</style>