<script>
import AppMainJumbo from './AppMainJumbo.vue'
import AppMainCourses from './AppMainCourses.vue'
import AppMainTutoring from './AppMainTutoring.vue'
import AppMainCompanionship from './AppMainCompanionship.vue'
import AppMainVerbatim from './AppMainVerbatim.vue'
import AppMainStas from './AppMainStats.vue'
import AppMainBlogs from './AppMainBlogs.vue'
import AppMainNewsletters from './AppMainNewsletters.vue'
export default {
    components: {

        AppMainJumbo,
        AppMainCourses,
        AppMainTutoring,
        AppMainCompanionship,
        AppMainVerbatim,
        AppMainStas,
        AppMainBlogs,
        AppMainNewsletters
    },
}
</script>
<!-- App che contiene tutti gli elementio del main divisi per titolo -->
<template>
    <AppMainJumbo />
    <AppMainCourses />
    <AppMainTutoring />
    <AppMainCompanionship />
    <AppMainVerbatim />
    <AppMainStas />
    <AppMainBlogs />
    <AppMainNewsletters />
</template>

<style scoped></style>