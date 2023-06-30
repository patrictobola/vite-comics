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
        <!-- Tag  -->
        <div class="tag">
            <span>Current series</span>
        </div>
        <div class="card-container">
            <div v-for="book in books" class="card">
                <ComicbookCard :books="book" />
            </div>
            <button>LOAD MORE</button>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../../assets/scss/vars' as *;

.container {
    position: relative;
}

span {
    color: white;
    font-size: 2rem;
    margin: 0;
    background-color: $blue;
    padding: 5px 10px;
}

.tag {
    position: absolute;
    top: -50px;
    left: 0px;
    transform: translate(0, -50%);
}

.card {
    width: calc(100% / 6 - 20px);
    padding: 10px;

}

.card-container {
    margin: 50px -10px 0 -10px;
    display: flex;
    flex-wrap: wrap;
}

ul {
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