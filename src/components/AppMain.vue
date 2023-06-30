<script>
import MainMenu from './MainMenu.vue';
export default {
    props: {
        menuLinks: Array
    },
    components: {
        MainMenu
    }
}
</script>
<template>
    <!-- Advertising section  -->
    <div class="adv">
        <div class="container">
            <h1>Content goes here</h1>
        </div>
    </div>
    <!-- Main menù section  -->
    <MainMenu :menuLinks="menuLinks" />
</template>



<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;

h1 {
    color: white;
}

.adv {
    height: 120px;
    @include flex(flex-start, center);
    background-color: $dark_gray;
}
</style>