<script>
export default {
    props: {
        books: Array,
    },
}
</script>

<template>
    <div v-for="book in books" :key="book.series" class="card">
        <div class="image">
            <img :src="book.thumb" :alt="book.series">
        </div>
        <div class="text">Price: {{ book.price }}</div>
        <div class="text">{{ book.series }}</div>
    </div>
</template>
<style lang="scss" scoped>
.card {
    width: calc(100% / 6 - 20px);
    padding: 10px;
}

.hover {
    background-color: white;
}

.text {
    color: white;
    padding-top: 5px;
    text-transform: uppercase;
}

.image {
    height: 200px;
    overflow: hidden;
}

img {
    display: block;
    width: 100%;
}
</style>