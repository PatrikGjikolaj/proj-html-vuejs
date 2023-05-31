<script>

export default {
    data() {
        return {
            courses: [
                {
                    photo: "../src/assets/course-02-480x298.jpg",
                    price: "$40.00",
                    description: "Learning to Write as a Professional Author",
                    time: "20 Lessons",
                    students: "50 Students"

                },
                {
                    photo: "../src/assets/stock-full-hd-03-480x298.jpg",
                    price: "Free",
                    description: "Custtomer-center Info-Tech Strategies",
                    time: "24 Lessons",
                    students: "769 Students"

                },
                {
                    photo: "../src/assets/stock-full-hd-04-480x298.jpg",
                    price: "$19.00",
                    description: "Open Programming Courses for Everyone: Phyton",
                    time: "17 Lessons",
                    students: "62 Students"

                },
                {
                    photo: "../src/assets/stock-full-hd-06-480x298.jpg",
                    price: "$26.00",
                    description: "Accademic Listening and Note-taking",
                    time: "14 Lessons",
                    students: "67 Students"

                },
                {
                    photo: "../src/assets/course-featured-image-01-480x298.jpg",
                    price: "$39.00",
                    description: "Master jQuery in a Short Period of Time",
                    time: "6 Lessons",
                    students: "51 Students"

                },
                {
                    photo: "../src/assets/stock-full-hd-05-480x298.jpg",
                    price: "$59.00",
                    description: "Introduction to Javascript for Beginners",
                    time: "14 Lessons",
                    students: "76 Students"

                },
            ]
        }
    },
}

</script>

<template>
    <div class="container-fluid bg_grey1 py-5">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center">
                    <h6 class="colorText">STIMULATED TO LEARN?</h6>
                    <h4 class="colorTitles">Featured Online Courses</h4>
                </div>
            </div>
            <div class="row py-5">
                <template v-for="course in courses">
                    <div class="col-6 py-3">
                        <div class="card border-0 bg_grey1">
                            <div class="row">
                                <div class="col-md-4">
                                    <img :src="course.photo" class="img-fluid rounded-circle" alt="">
                                </div>
                                <div class="col-md-8">
                                    <div class="card-body">
                                        <h5 class="card-title colorVipText fw-bold">{{ course.price }}</h5>
                                        <p class="card-text colorTitles">{{ course.description }}</p>
                                        <p class="card-text colorText"><small class="text-muted">
                                                {{ course.time }} {{ course.students }}
                                            </small></p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </template>
            </div>
            <div class="row">
                <div class="col-12 text-center">
                    <button type="button" class="btnCustom rounded">View all courses -></button>
                </div>
            </div>
        </div>
    </div>
</template>

<style  lang="scss" scoped>
img {
    aspect-ratio: 1;
    object-fit: cover;
}

.bg_grey1 {
    background-color: #f5f7fa;
}
</style>