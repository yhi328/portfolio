<template>
<v-app>
  <app-header></app-header>
  
 <router-view/>
  </v-app>
</template>

<script>
import AppHeader from "@/components/AppHeader"


export default {
  name: 'App',
  components:{
    AppHeader
  },
 
  data: () => ({
    //
  }),
};
</script>

<style scoped>
@import url("common/font/font.css");

*{font-family: 'Noto Sans KR', sans-serif;}

#app {
  width:100%;
  height: 100%;
}
</style>