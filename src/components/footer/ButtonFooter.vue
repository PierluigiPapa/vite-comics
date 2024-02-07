<script></script>

<template>
    <div>
        <div class="button">
            <a href="#">SIGN-UP NOW!</a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.button {
    padding: 12px;
    border: 2px solid $blue;

    a {
        color: white;
    }

    &:hover {
        cursor: pointer;
        background-color: $blue;
    }
}

</style>