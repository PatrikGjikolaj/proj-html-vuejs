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
            <div class="row gap-2">
                <div class="col-4 py-4">
                    <h6>ENJOYABLE INSIGHTS</h6>
                    <h4>Most Viewed Best Blogs</h4>
                    <ul class="py-4">
                        <template v-for="info in blogInfo">
                            <li class="py-2">{{ info }}</li>
                        </template>
                    </ul>
                </div>
                <template v-for="blog in blogs">
                    <div class="col-3">
                        <div class="card border-0">
                            <img :src="blog.pic" class="card-img-top" alt="">
                            <div class="card-body">
                                <p>{{ blog.job }}</p>
                                <h4>{{ blog.title }}</h4>
                                <span>{{ blog.date }} {{ blog.views }}</span>
                            </div>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>

<style scoped>
.bg_grey1 {
    background-color: #f5f7fa;
}
</style>