<script>
import FooterLinks from './FooterLinks.vue';
export default {
    components: {
        FooterLinks,
    }
}
</script>
<template>
    <div id="background">
        <div class="container">
            <div class="list-container">
                <div class="list-item">
                    <h2>DC COMICS</h2>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h2>SHOP</h2>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC collectibles</a></li>
                    </ul>
                </div>
                <div class="list-item">
                    <h2>DC</h2>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscription</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CBSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="list-item">
                    <h2>SITES</h2>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    <FooterLinks />
</template>
<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;

#background {
    background: no-repeat 80% 50% /500px url(../assets/img/dc-logo-bg.png), no-repeat center / 2000px url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
}

.list-container {
    padding: 40px 0;
    display: flex;
}

h2 {
    color: white;
    margin: 0;
}

a {
    color: #7c7c7c;
    font-size: 0.8rem;

    &:hover {
        color: $blue;
    }
}

.list-item {
    margin-right: 50px;
}
</style>

