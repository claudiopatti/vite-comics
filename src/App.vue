<script>
// 1) Importazione del componente 
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';




  export default {
  data() {
    return { 
        
    }
  },
  // 2) Dichiarizone del componente
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
}
</script>

<template>
    
    
    <AppHeader />

    <AppMain />

    <AppFooter />



</template>

<style lang="scss" >

@use 'assets/scss/partials/reset' as *;
@use 'assets/scss/main' as *;

</style>
