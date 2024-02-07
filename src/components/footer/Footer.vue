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
    <div class="container-footer">
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

.container-footer {
    max-width: 1520px;
    .content {
        margin: auto;
        display: flex;
        position: relative;
        overflow: hidden;
        padding: 30px 0;
        background-image: url('/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        .menu {
            z-index: 1;
        }

        .logo {
            position: absolute;
            right: 0;
            top: -40px;
        }
    }

    .contacts {
        background-color: $greydark;
    }
}
</style>