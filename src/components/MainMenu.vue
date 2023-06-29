<script>
export default {
    data() {
        return {
            mainLinks: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png',
                    url: '#'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png',
                    url: '#'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: 'buy-comics-subscriptions.png',
                    url: '#'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png',
                    url: '#'
                },
                {
                    text: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.svg',
                    url: '#'
                },
            ]
        }
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
                <li v-for="link in mainLinks"><a :href="link.url"><img :src="getImagePath(link.img)" alt="">{{ link.text
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