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
            <button>LOAD MORE</button>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../../assets/scss/vars' as *;

.card-container {
    margin: 50px -10px 0 -10px;
    display: flex;
    flex-wrap: wrap;
}

button {
    background-color: $blue;
    border: 0;
    border-radius: 5px;
    color: white;
    font-size: 1.2rem;
    padding: 10px 50px;
    margin: 20px auto;


    &:hover {
        background-color: #359cfd;
        cursor: pointer;
    }
}
</style>