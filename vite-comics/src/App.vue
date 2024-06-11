<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppBlueNav from "./components/AppBlueNav.vue";
import AppJumbotron from "./components/AppJumbotron.vue"


export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueNav,
    AppFooter,
    AppJumbotron,

  },
  
  data() {
    return {
    };
  }
};
</script>

<template>
    <AppHeader />
    <AppJumbotron/>
    <AppMain />
    <AppBlueNav />
    <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss'

</style>
