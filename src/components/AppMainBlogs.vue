<script>

export default {
    data() {
        return {
            blogs: [
                {
                    pic: "../src/assets/artist-blog-03-480x352.jpeg",
                    job: "ARTIST",
                    title: "Brush Strokes Energize Trees in Paintings",
                    date: "May 15, 2020",
                    views: "688 views"
                },
                {
                    pic: "../src/assets/artist-blog-01-480x352.jpg",
                    job: "ARTIST",
                    title: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    date: "May 15, 2020",
                    views: "603 views"
                },
            ],
            blogInfo: ["Became a Better Blogger: Content Planning", "Promoting Your Online Business on Pinterest", "Gamification and Game-Based Learning", "Designs an Online Course from Expert's Perspective", "Why Online Courses Are the Future of Education"]
        }
    },
}
</script>

<template>
    <div class="container-fluid bg_grey1 py-5">
        <div class="container py-5">
            <div class="row">
                <div class="col-6 py-4">
                    <h6 class="colorText">ENJOYABLE INSIGHTS</h6>
                    <h3 class="colorTitles">Most Viewed <span class="colorVipText fw-light">Best Blogs</span></h3>
                    <ul class="py-3 list-unstyled">
                        <template v-for="info in blogInfo">
                            <li class="py-2 colorTitles">&rarr; <small class=" ps-2 fw-bold"> {{ info }}</small>
                            </li>
                        </template>
                    </ul>
                </div>
                <template v-for="blog in blogs">
                    <div class="col-3">
                        <div class="card border-0">
                            <img :src="blog.pic" class="card-img-top" alt="">
                            <div class="card-body p-4">
                                <p class="colorText">{{ blog.job }}</p>
                                <h6 class="colorTitles">{{ blog.title }}</h6>
                                <small class="colorText">{{ blog.date }} {{ blog.views }}</small>
                            </div>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bg_grey3 {
    background-color: #f5f1ed;
}
</style>