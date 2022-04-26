<template>
  <main>
    <div class="container-fluid">
      <AboutComp />
    </div>
  </main>
</template>

<script>
import AboutComp from "@/components/About.vue";
export default {
  name: "MainCompenent",
  components: {
    AboutComp,
  },
};
</script>

<style scoped lang="scss">
main {
  margin: 100px 0;
}
</style>