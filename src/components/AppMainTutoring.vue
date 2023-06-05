<script>

export default {
    data() {
        return {
            benefits: [
                {
                    pic: "../src/assets/home-2-image-box-01.png",
                    title: "Customize Preferences",
                    description: "Learners are given the right to arrange and customize their study schedule and timetable based on preferences.",
                    link: "Start here"
                },
                {
                    pic: "../src/assets/about-us-02-image-box-02.png",
                    title: "Cloud Storage",
                    description: "You can store online lessons via online cloud or download to your device and revise lessons on the way",
                    link: "Get Free Quote"
                },
                {
                    pic: "../src/assets/home-2-image-box-03.png",
                    title: "Multimedia Channels",
                    description: "We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.",
                    link: "Start now"
                },
            ],
        }
    },
}
</script>
<!-- Sezione tutoring caricato tramite ciclo for su oggetto -->
<template>
    <div class="container-fluid bg_grey1 py-5">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center">
                    <h6 class="colorText">MAXCOACH AVAILABLE COURSES</h6>
                    <h4 class="colorTitles">Acces <span class="colorVipText fw-light">Smart Tutoring</span> Program For
                        Benefits.
                    </h4>
                </div>
            </div>
            <div class="row pt-5">
                <!-- Caricametno delle cards disponibili -->
                <template v-for="benefit in benefits">
                    <div class="col-lg-4 col-md-12">
                        <div class="card border-0">
                            <img :src="benefit.pic" class="card-img-top hCard" alt="">
                            <div class="card-body">
                                <h5 class="card-title colorTitles">{{ benefit.title }}</h5>
                                <p class="card-text colorText">{{ benefit.description }}</p>
                                <a href="" class="colorText PrimaryHov">{{ benefit.link }} &rarr;</a>
                            </div>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>

<style  lang="scss" scoped>
.hCard {
    width: 50%;
    aspect-ratio: 1;

}
</style>