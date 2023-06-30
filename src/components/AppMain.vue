<script>
import MainMenu from './mainsection/MainMenu.vue';
import MainComics from './mainsection/MainComics.vue';
export default {
    props: {
        links: Array
    },
    components: {
        MainMenu,
        MainComics,
    }
}
</script>
<template>
    <!-- Advertising section  -->
    <div class="jumbotron">
        <div class="container">
            <div class="tag">
                <span>Current series</span>
            </div>
        </div>
    </div>
    <!-- ComicBooks section  -->
    <MainComics />

    <!-- Main menù section  -->
    <MainMenu :links="links" />
</template>



<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;

span {
    color: white;
    font-size: 2rem;
    margin: 0;
    background-color: $blue;
    padding: 5px 10px;
}

.tag {
    position: absolute;
    bottom: 0px;
    left: 0px;
    transform: translate(0, 50%);
}

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