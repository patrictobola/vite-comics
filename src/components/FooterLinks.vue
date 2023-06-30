<script>
// Importo data con le  icone 
import footerIcons from '../assets/data/_footerIcons';
export default {
    data() {
        return {
            footerIcons
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
    <section>
        <div class="container">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div>
                <span>FOLLOW US</span>
                <ul>
                    <li v-for="icon in footerIcons">
                        <a href=""><img :src="getImagePath(icon.img)" alt=""></a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;

section {
    background-color: $gray;
    height: 120px;
}

ul {
    @include flex;
}

div {
    @include flex(flex-start, center);
    height: 100%;

}

span {
    color: $blue;
    margin-right: 20px;
    font-weight: 600;
}

button {
    background-color: inherit;
    border: 2px solid $blue;
    padding: 10px 20px;
    color: white;
    font-weight: 600;
    cursor: pointer;

    &:hover {
        color: $blue;
    }
}

.container {
    @include flex(space-between, center);
    height: 100%;

}

img {
    margin-right: 10px;
}
</style>