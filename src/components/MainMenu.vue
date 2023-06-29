<script>
export default {
    data() {
        return {
            mainLinks: [
                {
                    text: 'DIGITAL COMICS',
                    img: '../assets/img/buy-comics-digital-comics.png',
                    url: '#'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: '../assets/img/buy-comics-merchandise.png',
                    url: '#'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '../assets/img/buy-comics-subscriptions.png',
                    url: '#'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '../assets/img/buy-comics-shop-locator.png',
                    url: '#'
                },
                {
                    text: 'DC POWER VISA',
                    img: '@/assets/img/buy-dc-power-visa.svg',
                    url: '#'
                },
            ]
        }
    }
}
</script>
<template>
    <div>
        <div class="container">
            <ul>
                <li v-for="link in mainLinks"><a :href="link.url"><img :src="link.img" alt="">{{
                    link.text }}</a></li>
            </ul>
        </div>
    </div>
</template>
<style scoped>
div {
    height: 150px;
    display: flex;
    align-items: center;
    background-color: #0282f9;

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
}

img {
    height: 60px;
}
</style>