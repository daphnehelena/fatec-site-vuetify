<template>
  <v-app>
    <app-header/>
    <router-view />
    <app-footer/>
  </v-app>
</template>

<script>
import AppFooter from './components/AppFooter'
import AppHeader from './components/AppHeader'
export default {
  name: 'App',
  components:{
    AppFooter, AppHeader,
  }
}
</script>
<style>
template{
background-color: whitesmoke;
}
</style>