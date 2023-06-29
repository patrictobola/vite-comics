<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
// Supports weights 300-800
import '@fontsource-variable/open-sans';
export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  }
}
</script>
<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
.container {
  width: 1200px;
  margin: 0 auto;
}

body {
  font-family: 'Open Sans Variable', sans-serif;
  background-color: #000;
}

a {
  text-decoration: none;
}

li {
  list-style-type: none;
}
</style>