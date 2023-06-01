<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation, Pagination, Autoplay, EffectCoverflow } from 'swiper';

export default {
    data() {
        return {
            testimonials: [
                {
                    pic: "../src/assets/testimonial-avata-01.jpg",
                    title: "Customize Preferences",
                    description: "Learners are given the right to arrange and customize their study schedule and timetable based on preferences.",
                    link: "Start here ->"
                },
                {
                    pic: "../src/assets/testimonial-avata-02.jpg",
                    name: "MINA HOLLACE",
                    title: "High level of efficency and scientific teaching methods",
                    job: "/Freelancer",
                    description: "I am free to learn at my on space, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                },
                {
                    pic: "../src/assets/testimonial-avata-03.jpg",
                    name: "FLORENCE THEMES",
                    job: "/Multimedia Admin",
                    title: "It's a choice of quality for people with special needs",
                    description: "I'm very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me",
                },
                {
                    pic: "../src/assets/testimonial-avata-04.jpg",
                    name: "MADLEY PONDOR",
                    job: "IT Specialist",
                    title: "Professional team of specialists and passionate mentors ar rech",
                    description: "I need to get a certification for English proficiency and MAxCoach is my best choice. Their tutors are smart and professional when dealing with students",

                }
            ],
        }
    },
    components: {
        Swiper,
        SwiperSlide,
    },

    setup() {
        return {
            modules: [Navigation, Pagination, Autoplay, EffectCoverflow],
        }
    }
}
</script>

<template>
    <div class="container-fluid py-5 bg_grey1">
        <div class="row">
            <div class="col-12 text-center">
                <h6 class="colorText">GREAT WORDS ABOUT MAXCOACH</h6>
                <h3 class="colorTitles">Our <span class="colorVipText fw-light">top learners'</span> verbatim</h3>
            </div>
        </div>
        <div class="row py-5">
            <div class="col-12">
                <swiper :slidesPerView="3" :spaceBetween="50" :pagination="true" :mousewheel="true" :effect="'coverflow'"
                    :grabCursor="true" :centeredSlides="true" :autoplay="{ delay: 2000, }" :coverflowEffect="{
                        rotate: 10,
                        stretch: 0,
                        depth: 100,
                        modifier: 0.1,
                        slideShadows: true,
                    }" :modules="modules" class="mySwiper">
                    <template v-for="testimonial in testimonials">
                        <swiper-slide>
                            <div class="row card border-0 p-3">
                                <div class="list-group list-group-flush">
                                    <div class="col-12">
                                        <h5 class="colorTitles">{{ testimonial.title }}</h5>
                                        <p class="colorText">{{ testimonial.description }}</p>
                                    </div>
                                    <div class="list-group-item d-flex">
                                        <div class="col-2">
                                            <img :src="testimonial.pic" alt="" class="rounded-circle img-fluid">
                                        </div>
                                        <div class="col-10 p-3">
                                            <h6 class="colorTitles">{{ testimonial.name }}</h6>
                                            <small class="colorText">{{ testimonial.job }}</small>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </swiper-slide>
                    </template>
                </swiper>
            </div>
        </div>
        <div class="container">
            <div class="row">
                <div class="col-2 pt-5 rlt">
                    <span class="cerchio"></span>
                    <img src="../assets/maxcoach-shape-01.png" alt="">
                </div>
                <div class="col-8 text-center">
                    <h5 class="colorTitles">Start today for getting <span class="colorVipText fw-light">Online
                            Certification</span>
                    </h5>
                    <h3 class="colorTitles">You can be your own guiding star with our help!</h3>
                    <button type="button" class="btnCustom rounded my-3 px-5">View all courses -></button>
                </div>
                <div class="col-2 pt-5">
                    <img src="../assets/maxcoach-shape-02.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style  lang="scss" scoped>
.bg_grey2 {
    background-color: #f8f8f8;
}

.h100 {
    height: 100%;
}

.rlt {
    position: relative;
}

.cerchio {
    height: 40px;
    width: 40px;
    border: 5px solid #e6dcd2;
    border-radius: 50%;
    position: absolute;
    left: 5%;
    bottom: 75%;
}
</style>