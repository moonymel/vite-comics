<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueLine from './components/AppBlueLine.vue';
import AppFooter from './components/AppFooter.vue';
import AppCards from './components/AppCards.vue';


export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueLine,
    AppFooter,
    AppCards,

  }
}
</script>

<template lang="">
  <div>
    <AppHeader />
    <AppMain />
    <AppBlueLine />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/generals.scss' as *;
</style>