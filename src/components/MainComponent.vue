<template>
  <main class="container-fluid">
    <div>
      <AboutComp />
      <UpgradeSkill />
      <CoursesSection />
      <TestimonialSection />
    </div>
  </main>
</template>

<script>
import AboutComp from "@/components/About.vue";
import UpgradeSkill from "@/components/UpgradeSkill.vue";
import CoursesSection from "@/components/CoursesSection.vue";
import TestimonialSection from "@/components/Testimonials.vue";

export default {
  name: "MainCompenent",
  components: {
    AboutComp,
    UpgradeSkill,
    CoursesSection,
    TestimonialSection,
  },
};
</script>

<style scoped lang="scss">
main {
  margin: 100px 0;
}
</style>