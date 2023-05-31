<script>

export default {
    data() {
        return {
            linksExplore: ["Start here", "Blog", "About us", "Succes story", "Courses", "Contact us"],
            linksInformation: ["Membership", "Purchase guide", "Privacy policy", "Terms of services"],
        }
    },
}
</script>

<template>
    <div class="container-fluid py-5 bg_grey1">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <h4 class="colorTitles">Address</h4>
                    <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                    <p>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
                    <span>support@maxcoach.com</span>
                </div>
                <div class="col-4">
                    <h4 class="colorTitles">Explore</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkE in linksExplore">
                            <li><a href="" class="colorText textLinks">{{ linkE }}</a></li>
                        </template>
                    </ul>
                </div>
                <div class="col-2">
                    <h4 class="colorTitles">Information</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkI in linksInformation">
                            <li><a href="" class="colorText textLinks">{{ linkI }}</a></li>
                        </template>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
ul {
    list-style-type: none;
}

.textLinks {
    text-decoration: none;
}

.bg_grey1 {
    background-color: #f5f7fa;
}
</style>