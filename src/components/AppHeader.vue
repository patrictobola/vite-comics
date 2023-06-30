<script>
export default {
    props: {
        links: Array
    }
}
</script>
<template>
    <nav>
        <div id="navbar" class="container">

            <div class="logo">
                <a href=""><img src="../assets/img/dc-logo.png" alt=""></a>
            </div>
            <div class="links">
                <ul>
                    <li v-for="link in links" :key="link.text"><a :href="link.url">{{ link.text }}</a></li>
                </ul>

            </div>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;

nav {
    height: 100px;
    background-color: white;

}

#navbar {
    justify-content: space-between;
}

div {
    height: 100%;
    display: flex;
    align-items: center;
}

img {
    height: 80px;
}

ul {
    height: 100%;
    margin: 0;
}

li {
    list-style-type: none;
    padding: 0 10px;
    font-weight: 500;
    text-transform: uppercase;
    height: 100%;


}

a {
    color: black;
    height: 98%;
    display: flex;
    align-items: center;

    &:hover {
        color: $blue;
        border-bottom: 2px solid $blue;
    }
}

ul {
    display: flex;
}
</style>