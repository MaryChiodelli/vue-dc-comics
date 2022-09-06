<template>
    <div>
        <h4>{{ title }}</h4>
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            links: Array
        }
    }
</script>

<style lang="scss" scoped>
    h4 {
        font-size: 20px;
        font-weight: 700;
        line-height: 100%;
        margin-bottom: 1rem;
        text-transform: uppercase;
        color: #fff;
    }

    a {
        display: block;
        font-size: 12px;
        line-height: 165%;
        color: grey;
    }
</style>