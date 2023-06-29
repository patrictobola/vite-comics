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

div {
    height: 150px;
    display: flex;
    align-items: center;
    background-color: $blue;

}

ul {
    display: flex;
    justify-content: space-between;
    width: 100%;
    padding: 0;
    align-items: center;
}

li {
    display: flex;
}

a {
    color: white;
    display: flex;
    line-height: 60px;
}

img {
    height: 60px;
    padding-right: 10px;
}
</style>