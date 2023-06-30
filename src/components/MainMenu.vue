<script>
export default {
    props: {
        links: Array
    },
    methods: {
        getImagePath(image) {
            const url = new URL(`../assets/img/${image}`, import.meta.url)
            return url.href
        }
    }
}
</script>
<template>
    <div>
        <div class="container">
            <ul>
                <li v-for="link in links"><a :href="link.url"><img :src="getImagePath(link.img)" alt="">{{ link.text
                }}</a></li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;

div {
    height: 150px;
    @include flex(flex-start, center);
    background-color: $blue;

}

ul {
    @include flex(space-between, center);
    width: 100%;
    padding: 0;
}

li {
    display: flex;
}

a {
    color: white;
    display: flex;
    line-height: 60px;
    padding: 45px 10px;

    &:hover {
        background-color: rgba($color: #000000, $alpha: 0.1);
    }
}

img {
    height: 60px;
    padding-right: 10px;
}
</style>