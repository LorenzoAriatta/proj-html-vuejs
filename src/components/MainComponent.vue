<template>
  <main>
    <div class="container-fluid">
      <AboutComp />
      <UpgradeSkill />
    </div>
  </main>
</template>

<script>
import AboutComp from "@/components/About.vue";
import UpgradeSkill from "@/components/UpgradeSkill.vue";

export default {
  name: "MainCompenent",
  components: {
    AboutComp,
    UpgradeSkill,
  },
};
</script>

<style scoped lang="scss">
main {
  margin: 100px 0;
}
</style>