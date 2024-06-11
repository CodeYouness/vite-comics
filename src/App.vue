<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppShop from './components/AppShop.vue';


export default {
  data() {
    return {

    }
  },
  components:{
    AppHeader,
    AppMain,
    AppShop,
    AppFooter
  }
}
</script>

<template>

 <AppHeader/>
 <AppMain/>
 <AppShop/>
 <AppFooter/>

</template>

<style lang='scss'>
@use './styles/general.scss' as *

</style>
