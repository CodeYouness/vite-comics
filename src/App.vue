<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppJumbo from './components/AppJumbo.vue'


export default {
  data() {
    return {

    }
  },
  components:{
    AppHeader,
    AppMain,
    AppJumbo,
    AppFooter
  }
}
</script>

<template>
 <AppHeader/>
 <AppMain/>
 <AppJumbo/>
 <AppFooter/>
</template>

<style lang='scss'>
@use './styles/general.scss' as *

</style>
