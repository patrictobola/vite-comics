<script>
export default {

}
</script>


<template>
    <div class="container">
        <div class="card-container">
            <div class="card">
                <div class="image">
                    <img src="https://imgs.search.brave.com/OU2E3_3vA7flyv-SJ3TcFW1d99KDlp5ZfmW9ylLLFDo/rs:fit:1012:1200:1/g:ce/aHR0cHM6Ly9pMC53/cC5jb20vd3d3LnN1/cGVycG91dm9pci5j/b20vd3AtY29udGVu/dC91cGxvYWRzLzIw/MjAvMDcvQW1lcmlj/YW4tVmFtcGlyZS0x/OTc2LTAxLWNvdi1B/bGJ1cXVlcnF1ZS0y/MDIwLmpwZz9yZXNp/emU9MTAxMiUyQzE1/NTYmc3NsPTE"
                        alt="">
                </div>
                <div class="text">Asd</div>
            </div>

        </div>
    </div>
</template>


<style scoped>
.card-container {
    margin: 50px -10px;
    display: flex;
    flex-wrap: wrap;
}

.card {
    width: calc(100% / 6 - 20px);
    padding: 10px;
}

.text {
    color: white;
    padding-top: 5px;
    text-transform: uppercase;
}

.image {
    height: 200px;
    overflow: hidden;
}

img {
    display: block;
    width: 100%;
}
</style>