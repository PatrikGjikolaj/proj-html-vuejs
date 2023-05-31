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

<template>
    <div class="container-fluid">
        <div class="container">
            <div class="row">
                <template v-for="stat in stats">
                    <div class="col-3 text-center border-end py-5">
                        <h5>{{ stat.title }}</h5>
                        <h3>{{ stat.stat }}</h3>
                        <span>{{ stat.type }}</span>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>
<style scoped></style>