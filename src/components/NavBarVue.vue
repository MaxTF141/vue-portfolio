<template>
  <nav class="" :class="hover? 'navBar': 'NavBar'">
    <i class="bi bi-list menu-icon" @click="menuBar"></i>
    <div>
      <ul class="nav-items" v-if="hover">
        <router-link class="text-decoration-none nav_items" to="/"><i class="bi bi-house-door-fill"></i> Home</router-link>
        <router-link class="text-decoration-none nav_items" to="/about"><i class="bi bi-person-circle"></i> About</router-link> 
        <router-link class="text-decoration-none nav_items" to="/resume"><i class="bi bi-archive-fill"></i> Resume</router-link> 
        <router-link class="text-decoration-none nav_items" to="/projects"><i class="bi bi-file-earmark-code"></i> Projects</router-link>
        <router-link class="text-decoration-none nav_items" to="/testimonials"><i class="bi bi-chat-right-quote"></i> Testimonials</router-link> 
        <router-link class="text-decoration-none nav_items" to="/contact"><i class="bi bi-telephone-fill"></i> Contact Me</router-link> 
      </ul>
      <ul class="nav-items" v-else>
        <router-link class="text-decoration-none nav_items" to="/"><i class="bi bi-house-door-fill"></i></router-link>
        <router-link class="text-decoration-none nav_items" to="/about"><i class="bi bi-person-circle"></i></router-link> 
        <router-link class="text-decoration-none nav_items" to="/resume"><i class="bi bi-archive-fill"></i></router-link> 
        <router-link class="text-decoration-none nav_items" to="/projects"><i class="bi bi-file-earmark-code"></i></router-link>
        <router-link class="text-decoration-none nav_items" to="/testimonials"><i class="bi bi-chat-right-quote"></i></router-link> 
        <router-link class="text-decoration-none nav_items" to="/contact"><i class="bi bi-telephone-fill"></i></router-link> 
      </ul>
    </div>
  </nav>
</template>
<script>
export default {
  data() {
    return {
      hover: false
    }
  },
  methods:{
    menuBar(){
      this.hover = !this.hover
    }
  }
}
</script>
<style>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
 .NavBar{
  height: 100%;
  width: 50px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  overflow-x: hidden;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  padding-left: 5px;
}
 .navBar{
  height: 100%;
  width: 160px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  overflow-x: hidden;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  padding-left: 5px;
}
.nav-items {
  display: flex;
  flex-direction: column;
  padding:50px 0 0 0;
}
.nav_items {
  color: white;
  letter-spacing: 1px;
}
nav {
  background-color: #0c3047;
}
i{
  font-size: 2rem;
  color: white;
}
/* .menu-icon {
  padding-bottom: 100px;
} */
   
</style>