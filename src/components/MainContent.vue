<template>
    <main>
        <div class="hero">
            <!-- image -->
            <!-- Heading -->
        </div>
        <div class="series">
            <div class="container">
                <ProductCard />
            </div>
        </div>
    </main>
</template>

<script>
import ProductCard from './ProductCard.vue';

export default {
    components: {
        ProductCard
    }
}
</script>

<style lang="scss" scoped>
    main {
        .hero {
            height: 400px;
            background: url('../assets/jumbotron.jpg') top/cover no-repeat;
            background-color: #1c1c1c;
        }

        .series {
            background-color: #1c1c1c;
        }
    }
</style>