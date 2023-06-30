<script>
export default {
    props: {
        books: Object,
    },
}
</script>

<template>
    <div class="image">
        <img :src="books.thumb" :alt="books.series">
    </div>
    <div class="text">Price: {{ books.price }}</div>
    <div class="text">{{ books.series }}</div>
</template>
<style lang="scss" scoped>
.text {
    color: white;
    padding-top: 5px;
    text-transform: uppercase;
}

.image {
    height: 200px;
    overflow: hidden;

    &:hover {
        cursor: pointer;
    }
}

img {
    display: block;
    width: 100%;
}
</style>