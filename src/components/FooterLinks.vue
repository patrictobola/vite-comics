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
                    <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                    <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                    <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                    <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                    <li><img src="../assets/img/footer-periscope.png" alt=""></li>
                </ul>
            </div>
        </div>
    </section>
</template>
<style scoped>
section {
    background-color: #303030;
    height: 120px;
}

ul {
    display: flex;
}

div {
    display: flex;
    height: 100%;
    align-items: center;

}

span {
    color: blue;
    margin-right: 20px;
    font-weight: 600;
}

button {
    background-color: inherit;
    border: 2px solid blue;
    padding: 10px 20px;
    color: white;
    font-weight: 600;
    cursor: pointer;
}

.container {
    display: flex;
    height: 100%;
    align-items: center;
    justify-content: space-between;
}
</style>