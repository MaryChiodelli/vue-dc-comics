<template>
    <footer>
        <div class="features">
            <ul class="container feature-list">
                <li v-for="(feature, index) in features" :key="index" class="feature-item">
                    <img :src="feature.src" :alt="feature.text">
                    {{ feature.text }}
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
        <div class="footer-cta">
            <div class="container">
                <a class="button" href="#">Sign-up now!</a>
                <div class="socials">
                    <h3>Follow us</h3>
                    <ul class="social-list">
                        <li><a href="#"><img src="../assets/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    const features = [
        {
            src: require('../assets/buy-comics-digital-comics.png'),
            text: 'Digital comics'
        },
        {
            src: require('../assets/buy-comics-merchandise.png'),
            text: 'DC merchandise'
        },
        {
            src: require('../assets/buy-comics-subscriptions.png'),
            text: 'Subscription'
        },
        {
            src: require('../assets/buy-comics-shop-locator.png'),
            text: 'Comic shop locator'
        },
        {
            src: require('../assets/buy-dc-power-visa.svg'),
            text: 'DC power visa'
        }
    ]

    export default {
        data() {
            return {
                features: features
            }
        }
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

    .footer-cta {
        padding: 1.5rem 0;
        background-color: #303030;
        color: #fff;

        .container {
            display: flex;
            align-items: center;
            gap: 1rem;

            .button {
                display: block;
                padding: 8px 12px;
                border: 2px solid #0282f9;
                margin-right: auto;
                text-transform: uppercase;
            }
            
            .socials {
                display: contents;

                h3 {
                    color: #0282f9;
                    text-transform: uppercase;
                }

                .social-list {
                    display: flex;
                    gap: 1rem;
                }
            }
        }
    }
</style>