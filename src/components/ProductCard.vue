<template>
    <div class="card">
        <img :src="src" :alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>

<script>
export default {
    props: {
        src: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
    }

    h3 {
        font-size: 14px;
        text-transform: uppercase;
    }
</style>