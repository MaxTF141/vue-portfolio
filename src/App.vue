<template>
  <NavBarVue />
  <router-view/>
  <FooterVue />
</template>

<script>
import FooterVue from './components/FooterVue.vue';
import NavBarVue from './components/NavBarVue.vue';
  export default {
    components : {
      NavBarVue,
      FooterVue
    }
  }
</script>

<style>

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
