<template>
    <main>
        <div class="hero">
            <div class="container">
                <h2 class="hero-title">Current series</h2>
            </div>
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
            background: url('../assets/jumbotron.jpg') top/cover no-repeat;
            background-color: #1c1c1c;

            .container {
                height: 400px;
                position: relative;
            }

            .hero-title {
                padding: 0.5rem 1rem;
                position: absolute;
                bottom: 0;
                left: 1rem;
                transform: translateY(+50%);
                background-color: #0282f9;
                color: #fff;
                text-transform: uppercase;
            }
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