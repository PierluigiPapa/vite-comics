<script>
import Header from './components/header/Header.vue';
import Jumbotron from './components/jumbotron/Jumbotron.vue';
import MainMenu from './components/main/MainMenu.vue';

export default {
  components: {
    Header,
    Jumbotron,
    MainMenu,
  }
}

</script>

<template>

<Header></Header>
<Jumbotron></Jumbotron>
<MainMenu></MainMenu>

</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
