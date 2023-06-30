<script>
// Importo componenti 
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
// Importo il font 
import '@fontsource-variable/open-sans';
// Importo i data 
// import MenuLinks from './assets/data/MenuLinks.js';

export default {
  // props: {
  //   MenuLinks
  // },
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  },
  data() {
    return {
      menuLinks: [
        {
          text: 'DIGITAL COMICS',
          img: 'buy-comics-digital-comics.png',
          url: '#'
        },
        {
          text: 'DC MERCHANDISE',
          img: 'buy-comics-merchandise.png',
          url: '#'
        },
        {
          text: 'SUBSCRIPTION',
          img: 'buy-comics-subscriptions.png',
          url: '#'
        },
        {
          text: 'COMIC SHOP LOCATOR',
          img: 'buy-comics-shop-locator.png',
          url: '#'
        },
        {
          text: 'DC POWER VISA',
          img: 'buy-dc-power-visa.svg',
          url: '#'
        },
      ]
    }

  }
}
</script>
<template>
  <AppHeader />
  <AppMain :menuLinks="menuLinks" />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>