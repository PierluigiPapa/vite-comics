<script>
import Header from './components/header/Header.vue';
import Jumbotron from './components/jumbotron/Jumbotron.vue';

export default {
  components: {
    Header,
    Jumbotron,
  }
}

</script>

<template>

<Header></Header>
<Jumbotron></Jumbotron>

</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
