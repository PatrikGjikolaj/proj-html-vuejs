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
    <div>
        <span class="abs text-center colorText p-3 border rounded">
            <i class="fa-solid fa-ruler-combined pb-3 PrimaryHov"></i>
            <i class="fa-solid fa-life-ring pb-3 PrimaryHov"></i>
            <i class="fa-solid fa-book pb-3 PrimaryHov"></i>
            <i class="fa-solid fa-cart-shopping PrimaryHov"></i>
        </span>
        <AppMainJumbo />
        <AppMainCourses />
        <AppMainTutoring />
        <AppMainCompanionship />
        <AppMainVerbatim />
        <AppMainStas />
        <AppMainBlogs />
        <AppMainNewsletters />
    </div>
</template>

<style scoped>
.abs {
    position: fixed;
    left: calc(100% - 45px);
    top: 30%;
}
</style>