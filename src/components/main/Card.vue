<script>
export default {
    name: 'Card',
    props: {
        image: String,
        title: String,
    },
}
</script>

<template>
    <div class="card">
        <div class="img-card">
            <img :src="image" :alt="title">
        </div>
        <div class="text">{{ title }}</div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.card {
    margin: 10px;
    width: calc(100% / 6 - 20px);
    display: flex;
    flex-direction: column;

    .img-card {
        width: 100%;
        img {
            width: 100%;
            aspect-ratio: 3/4;
        }
    }
}



</style>