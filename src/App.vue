<script>
import Header from './components/header/Header.vue';
import Jumbotron from './components/jumbotron/Jumbotron.vue';
import Main from './components/main/Main.vue';
import Footer from './components/footer/Footer.vue';

export default {
  components: {
    Header,
    Jumbotron,
    Main,
    Footer,
  }
}

</script>

<template>

<Header></Header>

<Jumbotron></Jumbotron>

<main>
  <Main></Main>
</main>

<footer>
  <Footer></Footer>
</footer>


</template>

<style lang="scss">
@use "./styles/general.scss";
</style>