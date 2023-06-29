<script>
export default {
    data() {
        return {
            NavbarLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]

        }
    }
}
</script>
<template>
    <nav>
        <div id="navbar" class="container">

            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="links">
                <ul>
                    <li v-for="link in this.NavbarLinks" :key="link.text"><a :href="link.url">{{ link.text }}</a></li>
                </ul>

            </div>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
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
        color: lightblue;
        border-bottom: 2px solid lightblue;
    }
}

ul {
    display: flex;
}
</style>