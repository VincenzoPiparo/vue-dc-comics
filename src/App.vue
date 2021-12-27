<template>
  <div id="app">
    <Header />
    <Main />
    <Banner />
    <PreFooter />
     <PostFooter />
  </div>
</template>

<script>

import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Banner from "./components/Banner.vue";
import PreFooter from "./components/PreFooter.vue";
import PostFooter from "./components/PostFooter.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Banner,
    PreFooter,
    PostFooter,
  },
};
</script>

<style lang="scss">
@import './styles/general.scss';
</style>
