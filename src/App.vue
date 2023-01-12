<template>
  <NavBarVue />
  <router-view>
      
  </router-view>
  <FooterVue />
</template>

<script>
import FooterVue from './components/FooterVue.vue';
import NavBarVue from './components/NavBarVue.vue';
  export default {
    components : {
      NavBarVue,
      FooterVue
    },
  }
</script>

<style>
*,
*::after,
*:before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

nav a.router-link-exact-active {
  color: #42b983;
}

footer {
    background-color: #0c3047;
}

</style>
