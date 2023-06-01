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
    <div class="container-fluid pt-5 bg_grey1">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <h4>Address</h4>
                    <p class="colorText">382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                    <p class="colorText">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
                    <a class="colorText greenHov">support@maxcoach.com</a>
                    <div class="py-5">
                        <a href=""><i class="fa-brands fa-square-facebook logoLinks greenHov"></i></a>
                        <a href=""><i class="fa-brands fa-twitter logoLinks px-4 greenHov"></i></a>
                        <a href=""><i class="fa-brands fa-instagram logoLinks greenHov"></i></a>
                        <a href=""><i class="fa-brands fa-linkedin logoLinks greenHov px-4"></i></a>
                    </div>
                </div>
                <div class="col-4">
                    <h4>Explore</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkE in linksExplore">
                            <li><a href="" class="colorText greenHov">{{ linkE }}</a></li>
                        </template>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>Information</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkI in linksInformation">
                            <li><a href="" class="colorText greenHov">{{ linkI }}</a></li>
                        </template>
                    </ul>
                </div>
            </div>
        </div>
        <div class="row p-3">
            <div class="col-10 offset-1 text-center colorText abs">
                <p>© 2020 Maxcoach. All Rights Reserved</p>
            </div>
            <div class="col-1">
                <a class=" footBtn border-0 p-3 colorText" href="navbar"><i class="fa-solid fa-arrow-up m-auto"></i></a>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

ul {
    list-style-type: none;
}

.greenHov:hover {
    color: $ColorPrimary;
}

.logoLinks {
    font-size: 30px;
    color: #696969;
}

.footBtn {
    background-color: $ColorPrimary;
    border-radius: 50%;
    height: 50px;
    width: 50px;
    display: flex;
    align-items: center;
}
</style>