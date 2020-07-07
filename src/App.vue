<template>
<div id="app">

    <!-- Navigation -->
    <navigation></navigation>

    <!-- Header -->
    <Header></Header>

    <!-- About -->
    <app-about></app-about>

    <!-- Services -->

    <!-- Portfolio Grid -->
    <app-portfolio></app-portfolio>

    <!-- Contact -->
<app-contact></app-contact>
    <!-- Footer -->
    <Footer></Footer>

    <!-- Portfolio Modals -->

  </div>
</template>

<script>
import Navigation from './components/Navigation.vue';
import Header from './components/Header.vue';
// import Services from './components/Services.vue';
import Portfolio from './components/Portfolio.vue';
import About from './components/About.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'app',
  components: {
    Navigation,
    Header,
    Footer,
    'app-portfolio': Portfolio,
    // 'app-services': Services,
    'app-about': About,
    'app-contact': Contact,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  background: black;
}
</style>
