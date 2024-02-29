<script>
import AppHeader from './components/AppHeader.vue';
import AppContent from './components/AppContent.vue';
import AppBodyNav from './components/AppBodyNav.vue';
import AppTopFooter from './components/AppTopFooter.vue';
import AppBottomFooter from './components/AppBottomFooter.vue';
export default{

  components:{
   AppHeader,
   AppContent,
   AppBodyNav,
   AppTopFooter,
   AppBottomFooter
  },

  data(){
    return{

    }
  }

}
</script>

<template>
<AppHeader></AppHeader>
<AppContent></AppContent>
<AppBodyNav></AppBodyNav>
<AppTopFooter></AppTopFooter>
<AppBottomFooter></AppBottomFooter>

</template>

<style>

</style>