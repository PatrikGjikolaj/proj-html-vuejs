


<template>
    <div class="container my-5">
        <div class="row">
            <div class="col-3 pt-5 rlt">
                <span class="cerchio"></span>
            </div>
            <div class="col-6 text-center px-2">
                <h3 class="colorTitles">Subscibe <span class="colorVipText fw-light">Newsletters</span></h3>
                <h6 class="colorText px-5">Enter your email address to register to our newsletter subscriptions deliverd on
                    a regular basis!</h6>
                <div class="input-group p-5">
                    <input type="text" class="form-control" placeholder="Enter your email" aria-label="Recipient's username"
                        aria-describedby="basic-addon2">
                    <span class="input-group-btn btnCustom rounded-end p-2" id="basic-addon2">Subscribe</span>
                </div>
            </div>
            <div class="col-3 pt-5 text-end">
                <img src="../assets/maxcoach-shape-02.png" alt="">
            </div>
        </div>
    </div>
</template>
<style  lang="scss" scoped>
@use '../styles/variables.scss' as *;

.rlt {
    position: relative;
}

.cerchio {
    height: 40px;
    width: 40px;
    border: 5px solid $ColorPrimary;
    border-radius: 50%;
    position: absolute;
    left: -10%;
    bottom: 50%;
}
</style>