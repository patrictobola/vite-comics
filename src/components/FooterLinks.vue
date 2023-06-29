<script>
export default {

}
</script>
<template>
    <section>
        <div class="container">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div>
                <span>FOLLOW US</span>
                <ul>
                    <li><a href="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </a>
                    </li>
                    <li><a href="">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </a>
                    </li>
                    <li><a href="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </a>
                    </li>
                    <li><a href="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </a>
                    </li>
                    <li><a href="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;
@use '../assets/scss/_mixins.scss' as *;

section {
    background-color: $gray;
    height: 120px;
}

ul {
    @include flex;
}

div {
    @include flex(flex-start, center);
    height: 100%;

}

span {
    color: $blue;
    margin-right: 20px;
    font-weight: 600;
}

button {
    background-color: inherit;
    border: 2px solid $blue;
    padding: 10px 20px;
    color: white;
    font-weight: 600;
    cursor: pointer;
}

.container {
    @include flex(space-between, center);
    height: 100%;
}

img {
    margin-right: 10px;
}
</style>