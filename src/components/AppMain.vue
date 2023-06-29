<script>
import MainMenu from './MainMenu.vue';
export default {
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
    <MainMenu />
</template>
<style scoped>
h1 {
    color: white;
}

.adv {
    height: 120px;
    display: flex;
    align-items: center;
    background-color: slategray;
}
</style>