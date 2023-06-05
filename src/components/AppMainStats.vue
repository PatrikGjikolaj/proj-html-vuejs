<script>

export default {
    data() {
        return {
            stats: [
                {
                    title: "Successfully trained",
                    stat: "1790",
                    type: "ENROLLED LEARNERS"
                },
                {
                    title: "Proudly Received",
                    stat: "19",
                    type: "COUNTRIWIDE AWARDS"
                },
                {
                    title: "Firmly Established",
                    stat: "24",
                    type: "LOCAL BRANCHES"
                },
                {
                    title: "Getting Featured on",
                    stat: "1090",
                    type: "BLOCK POSTS"
                },
            ],
        }
    },
}
</script>
<!-- Sezione delle statistiche con caricamento tramite ciclo for su oggetto -->
<template>
    <div class="container-fluid">
        <div class="container">
            <div class="row">
                <template v-for="stat in stats">
                    <div class="col-3 text-center border-end border-start p-5">
                        <h5 class="colorTitles px-5">{{ stat.title }}</h5>
                        <h2 class="colorVipText fw-bold">{{ stat.stat }}</h2>
                        <small class="colorText fw-bold">{{ stat.type }}</small>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>
<style  lang="scss" scoped></style>