<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="DC Comics logo">
            </div>
            <nav class="nav">
                <ul class="nav-list">
                    <li v-for="(link, index) in links" :key="index" class="nav-item">
                        <a class="nav-link" href="link.href">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    const links = [
        {
            href: '#',
            text: 'characters',
            active: false
        },
        {
            href: '#',
            text: 'comics',
            active: true
        },
        {
            href: '#',
            text: 'movies',
            active: false
        },
        {
            href: '#',
            text: 'tv',
            active: false
        },
        {
            href: '#',
            text: 'games',
            active: false
        },
        {
            href: '#',
            text: 'collectibles',
            active: false
        },
        {
            href: '#',
            text: 'videos',
            active: false
        },
        {
            href: '#',
            text: 'fans',
            active: false
        },
        {
            href: '#',
            text: 'news',
            active: false
        },
        {
            href: '#',
            text: 'shop',
            active: false
        }
    ]

    export default {
        data() {
            return {
                links: links
            }
        }
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
            .nav-list {
                display: flex;
                align-items: center;
                gap: 1.5rem;
            }

            .nav-link {
                display: block;
                line-height: 3rem;
                border-bottom: 4px solid #fff;
                text-transform: uppercase;
            }


            .nav-link:hover {
                border-color: #0282f9;
            }
        }
    }
</style>