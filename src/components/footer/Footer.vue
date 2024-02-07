<script>
import LogoFooter from './LogoFooter.vue';
import MenuFooter from './MenuFooter.vue';
import EndFooter from './EndFooter.vue';

export default {
  components: {
    LogoFooter,
    MenuFooter,
    EndFooter,
  }
}
</script>

<template>
    <div class="container">
        <div class="content">
            <div class="menu">
                <MenuFooter></MenuFooter>
            </div>

            <div class="logo">
                <LogoFooter></LogoFooter>
            </div>
        </div>
        <div class="contacts">
            <EndFooter></EndFooter>
        </div>
    </div>
    
</template>
  
<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;



</style>