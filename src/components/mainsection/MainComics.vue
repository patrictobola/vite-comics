<script>
import ComicbookCard from './ComicbookCard.vue';
export default {
    components: {
        ComicbookCard,
    },
    props: {
        books: Array,
    }
}
</script>


<template>
    <div class="container">
        <div class="card-container">
            <ComicbookCard :books="books" />
        </div>
    </div>
</template>


<style scoped>
.card-container {
    margin: 50px -10px;
    display: flex;
    flex-wrap: wrap;
}
</style>