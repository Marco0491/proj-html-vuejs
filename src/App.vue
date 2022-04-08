<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Jumbotron from './components/Jumbotron.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import './assets/styles/style.scss';
@import '~bootstrap/scss/bootstrap.scss';
</style>
