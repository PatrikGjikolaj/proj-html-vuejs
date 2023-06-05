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
<!-- Sezione del footer con i link e vari hover -->
<template>
    <div class="container-fluid pt-5 bg_grey1">
        <div class="container">
            <div class="row">
                <!-- Sezione statica dell'indirizzo -->
                <div class="col-md-6">
                    <h4>Address</h4>
                    <p class="colorText">382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                    <p class="colorText">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
                    <a class="colorText PrimaryHov">support@maxcoach.com</a>
                    <div class="py-5">
                        <a href=""><i class="fa-brands fa-square-facebook logoLinks colorText PrimaryHov"></i></a>
                        <a href=""><i class="fa-brands fa-twitter px-4 logoLinks colorText PrimaryHov"></i></a>
                        <a href=""><i class="fa-brands fa-instagram logoLinks colorText PrimaryHov"></i></a>
                        <a href=""><i class="fa-brands fa-linkedin logoLinks colorText PrimaryHov px-4"></i></a>
                    </div>
                </div>
                <!-- Sezione dei link caricati tramite cicli for su array -->
                <div class="col-4">
                    <h4>Explore</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkE in linksExplore">
                            <li><a href="" class="colorText PrimaryHov">{{ linkE }}</a></li>
                        </template>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>Information</h4>
                    <ul class="m-0 px-0">
                        <template v-for="linkI in linksInformation">
                            <li><a href="" class="colorText PrimaryHov">{{ linkI }}</a></li>
                        </template>
                    </ul>
                </div>
            </div>
        </div>
        <div class="row p-3">
            <div class="col-md-10 offset-1 text-center colorText abs">
                <p>© 2020 Maxcoach. All Rights Reserved</p>
            </div>
            <div class="col-md-1">
                <a class=" footBtn border-0 p-3 colorText btnCustom" href="navbar"><i
                        class="fa-solid fa-arrow-up m-auto text-light"></i></a>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/variables.scss' as *;

ul {
    list-style-type: none;
}


.logoLinks {
    font-size: 30px;
    // color: #696969;
}

.footBtn {
    border-radius: 50%;
    height: 50px;
    width: 50px;
    display: flex;
    align-items: center;
}
</style>