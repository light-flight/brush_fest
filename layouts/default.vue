<template>
  <v-app>
    <Navbar />
    <nuxt />
    <Footer />
  </v-app>
</template>

<script>
  import Navbar from '~/components/Navbar.vue';
  import Footer from '~/components/Footer.vue';

  export default {
    components: {
      Navbar,
      Footer
    }
  }
</script>

<style>
html {
  font-size: 100%;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
</style>
