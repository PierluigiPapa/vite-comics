<script>
import MainMenu from './MainMenu.vue';
import SectionCards from './SectionCards.vue';

export default {
  components: {
    MainMenu,
    SectionCards,
  }
}
</script>

<template>

    <section>
      <SectionCards></SectionCards>
    </section>

    <section>
      <MainMenu></MainMenu>
    </section>

</template>

<style lang="scss" scoped>

</style>