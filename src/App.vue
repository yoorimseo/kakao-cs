<template>
  <div>
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style>
body {
  width: 100vw;
  height: 100vh;
  margin: 0;
  background-color: white;
  overflow-x: hidden;
}
#app {
  width: 100vw;
  min-width: 63.75em;
  height: 100vh;
  margin: 0;
}
a {
  text-decoration: none;
  color: black;
}
</style>
