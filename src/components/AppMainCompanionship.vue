<script>

</script>

<template>
    <div class="container-fluid py-5 imgBackJumbo bg_custom">
        <div class="container py-5">
            <div class="row align-items-center">
                <div class="col-7 text-center">
                    <div class="posR rlt">
                        <img src="../assets/home-2-popup-video-poster.jpg" alt="" class="imgJumbo rounded">
                        <img src="../assets/icon-youtube-play.png" alt="" class="posA">
                        <span class="cerchio"></span>
                        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="202px"
                            viewBox="0 0 200 202" class="svg">
                            <path class="elementor-shape-fill"
                                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
                            </path>
                        </svg>
                    </div>
                </div>
                <div class="col-5 d-flex flex-column p-5 gap-4">
                    <h6 class="colorText">GET STARTED <span class="colorTitles">EFFORTLESSLY</span>
                    </h6>
                    <h1 class="colorTitles">Enjoy Our <span class="colorVipText fw-light">Companionship</span></h1>
                    <p class="colorText">Sneek peek into what has in store for you on our online teaching and mentoring
                        portal. Seek for some
                        hidden hints of early-bird rewards as well</p>
                    <a href="" class="colorVipText fw-bold">Download free guidebook &rarr;</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss';

.imgJumbo {
    width: 90%;
}

.posR {
    position: relative;
}

.posA {
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    margin: auto;
}

.imgBackJumbo {
    background-image: url(../assets/maxcoach-shape-05-150x150.png), url(../assets/maxcoach-shape-07-100x100.png);
    background-position: 5% 30%, 52% 95%;
    background-repeat: no-repeat;
}

.rlt {
    position: relative;
}

.svg {
    position: absolute;
    right: 80%;
    bottom: 80%;
    z-index: -1;
    fill: #e5c791;
}

.cerchio {
    height: 70px;
    width: 70px;
    border: 10px solid #ecc5ab;
    border-radius: 50%;
    position: absolute;
    left: 102%;
    bottom: 90%;
}
</style>