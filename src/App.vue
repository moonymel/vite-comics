<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueLine from './components/AppBlueLine.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppBlueLine,

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

@import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');


h1 {
  font-family: Oswald;
}
</style>