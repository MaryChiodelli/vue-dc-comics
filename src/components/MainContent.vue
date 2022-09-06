<template>
    <main>
        <div class="hero">
            <!-- image -->
            <!-- Heading -->
        </div>
        <div class="series">
            <div class="container serie-list">
                <ProductCard class="serie-item" v-for="(serie, index) in series" :key="index" :src="serie.thumb" :title="serie.series" />
            </div>
            <div class="container cta">
                <a href="#">Load More</a>
            </div>
        </div>
    </main>
</template>

<script>
    import ProductCard from './ProductCard.vue';
    import series from '../dc-comics.js';

    export default {
        components: {
            ProductCard
        },
        data() {
            return {
                series: series
            }
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
            padding: 3rem 0;
            color: #fff;
            background-color: #1c1c1c;

            .serie-list {
                margin-bottom: 1.5rem;
                display: flex;
                flex-wrap: wrap;
                gap: 1.5rem;

                .serie-item {
                    flex-basis: 185px;
                    flex-grow: 1;
                    padding: 0 0.75rem;
                }
            }


            .cta {
                text-align: center;

                a {
                    display: inline-block;
                    padding: 0.25rem 2rem;
                    line-height: 1.5rem;
                    background-color: #0282f9;
                }
            }
        }
    }
</style>