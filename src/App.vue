<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/projects">Projects</router-link> |
    <router-link to="/testimonials">Testimonials</router-link> |
    <router-link to="/contact">Contacts</router-link> |
  </nav>
  <router-view />
  <footerVue />
</template>

<script>
import footer from "./components/footer.vue";
import footerVue from "./components/footer.vue";

export default {
  components: { footerVue },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  background-color: black;
}

nav a {
  font-weight: bold;
  color:whitesmoke;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
