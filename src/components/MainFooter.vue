<template>
    <footer>
        <div class="features">
            <ul class="container feature-list">
                <li class="feature-item">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    Digital comics
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                    DC merchandise
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                    Subscription
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                    Comic shop locator
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                    DC power visa
                </li>
            </ul>
        </div>
        <div class="container"></div>
        <div class="container"></div>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .features {
        padding: 3rem 0;
        background-color: #0282f9;

        .feature-list {
            display: flex;
            flex-wrap: wrap;
        }

        .feature-item {
            flex-basis: 0;
            flex-grow: 1;

            display: flex;
            justify-content: center;
            align-items: center;
            gap: 12px;
            color: #fff;
            text-transform: uppercase;

            img {
                width: 60px;
                aspect-ratio: 1 / 1;
                object-fit: contain;
            }
        }
    }
</style>