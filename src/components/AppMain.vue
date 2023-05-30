<script>
import AppMainJumbo from './AppMainJumbo.vue'
import AppMainCourses from './AppMainCourses.vue'
import AppMainTutoring from './AppMainTutoring.vue'
import AppMainCompanionship from './AppMainCompanionship.vue'
import AppMainVerbatim from './AppMainVerbatim.vue'
export default {
    components: {

        AppMainJumbo,
        AppMainCourses,
        AppMainTutoring,
        AppMainCompanionship,
        AppMainVerbatim
    },
}
</script>

<template>
    <AppMainJumbo />
    <AppMainCourses />
    <AppMainTutoring />
    <AppMainCompanionship />
    <AppMainVerbatim />
</template>

<style scoped></style>