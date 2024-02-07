<script>
import ButtonFooter from './ButtonFooter.vue';
import SocialFooter from './SocialFooter.vue';
 
export default {
  components: {
    ButtonFooter,
    SocialFooter,
  }
}
</script>

<template>
    <div class="container">
        <div class="content">
            <div class="button">
                <ButtonFooter></ButtonFooter>
            </div>
            <div class="social">
                <SocialFooter></SocialFooter>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.container {
    max-width: 1520px;
    margin: auto;
    .content {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 30px;
    }
}
</style>