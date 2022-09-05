<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="DC Comics logo">
            </div>
            <nav class="nav">
                <ul class="nav-list">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Characters</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="#">Comics</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Movies</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Tv</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Games</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Collectibles</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Videos</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Fans</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">News</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Shop</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    header {
        padding: 1rem 0;
        background-color: #fff;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 1rem;
        }

        .logo {
            width: 80px;
            height: 80px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }

        .nav {
            &-list {
                display: flex;
                align-items: center;
                gap: 1rem;
            }

            &-item.active {
                border-bottom: 4px solid #0282f9;
            }
            
            &-link {
                padding: 0 12px;
                line-height: 1.5rem;
                text-transform: uppercase;
            }
        }
    }
</style>