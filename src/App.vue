<template>
  <div id="app">
    <Header />
    <Main />
    <Banner />
    <PreFooter />
  </div>
</template>

<script>

import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Banner from "./components/Banner.vue";
import PreFooter from "./components/PreFooter.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Banner,
    PreFooter,
  },
};
</script>

<style lang="scss">
@import './styles/general.scss';
</style>
