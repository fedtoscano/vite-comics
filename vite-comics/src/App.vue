<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppBlueNav from "./components/AppBlueNav.vue"

export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueNav,
    AppFooter,
  },
  data() {
    return {
    };
  }
};
</script>

<template>
    <AppHeader />
    <AppMain />
    <AppBlueNav />
    <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss'

</style>
