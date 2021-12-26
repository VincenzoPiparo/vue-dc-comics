<template>
  <div id="app">
    <Header />
    <Main/>
    <Banner/>
  </div>
</template>

<script>

import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Banner from "./components/Banner.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Banner,
  },
};
</script>

<style lang="scss">
@import './styles/general.scss';
</style>
