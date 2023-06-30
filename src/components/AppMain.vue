<script>
import MainMenu from './mainsection/MainMenu.vue';
import ComicbookSection from './mainsection/ComicbookSection.vue';
export default {
    props: {
        links: Array,
        books: Array
    },
    components: {
        MainMenu,
        ComicbookSection,
    }
}
</script>
<template>
    <!-- Advertising section  -->
    <div class="jumbotron">
        <div class="container">

        </div>
    </div>
    <!-- ComicBooks section  -->
    <ComicbookSection :books="books" />

    <!-- Main menù section  -->
    <MainMenu :links="links" />
</template>



<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;



.container {
    height: 100%;
    position: relative;
}

.jumbotron {
    height: 400px;
    @include flex(flex-start, center);
    background: no-repeat url(../assets/img/jumbotron.jpg);
}
</style>