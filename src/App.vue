<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default{
    name: 'App',
    components: {
      AppHeader,//componente dell'header
      AppMain, //componente del main
      AppFooter //componente del footer
    }
}

</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6{
  color: $primary;
}

</style>
