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
        <div class="nav">
            <div class="container">
                <div>
                    <h3>DC comics</h3>
                    <ul>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                    </ul>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                    </ul>
                </div>
                <div>
                    <h3>Sites</h3>
                    <ul>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                        <li><a href="#">Link</a></li>
                    </ul>
                </div>
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
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

    .nav {
        padding: 3rem 0;
        background: url('../assets/footer-bg.jpg') center/cover no-repeat #1c1c1c;
        color: #fff;
        overflow: hidden;

        .container {
            display: flex;
            gap: 1.5em;
            position: relative;

            img {
                width: 560px;
                margin-left: auto;
                position: absolute;
                top: 50%;
                right: 0;
                transform: translateY(-50%);
            }
        }
    }
</style>