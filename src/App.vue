<template>
  <div id="app">
    <Header />
    <JumboComponent />
    <MainCompenent />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import JumboComponent from "@/components/JumboComponent.vue";
import MainCompenent from "@/components/MainComponent.vue";

export default {
  name: "App",
  components: {
    Header,
    JumboComponent,
    MainCompenent,
  },
};
</script>

<style lang="scss">
@import "@/style/general.scss";
#app {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}
</style>
