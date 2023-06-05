<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  components: {

    AppHeader,
    AppMain,
    AppFooter

  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/variables.scss';

* {
  scrollbar-width: auto;
  scrollbar-color: ColorPrimary;
}

*::-webkit-scrollbar {
  width: 20px;
}

*::-webkit-scrollbar-track {
  background: #ffffff;
}

*::-webkit-scrollbar-thumb {
  background-color: #ef6f31;
  border-radius: 10px;
  border: 3px solid #ffffff;
}
</style>
