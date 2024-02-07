<script>
import Header from './components/header/Header.vue';
import Jumbotron from './components/jumbotron/Jumbotron.vue';
import MainMenu from './components/main/MainMenu.vue';
import Footer from './components/footer/Footer.vue';

export default {
  components: {
    Header,
    Jumbotron,
    MainMenu,
    Footer,
  }
}

</script>

<template>

<Header></Header>

<Jumbotron></Jumbotron>

<MainMenu></MainMenu>

<footer>
  <Footer></Footer>
</footer>


</template>

<style lang="scss">
@use "./styles/general.scss";
</style>