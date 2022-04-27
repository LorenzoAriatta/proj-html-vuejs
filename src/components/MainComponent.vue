<template>
  <main>
    <div>
      <AboutComp />
      <UpgradeSkill />
      <CoursesSection />
      <TestimonialSection />
      <CoachSection />
      <BlogSection />
    </div>
  </main>
</template>

<script>
import AboutComp from "@/components/About.vue";
import UpgradeSkill from "@/components/UpgradeSkill.vue";
import CoursesSection from "@/components/CoursesSection.vue";
import TestimonialSection from "@/components/Testimonials.vue";
import CoachSection from "@/components/CoachSection.vue";
import BlogSection from "@/components/BlogSection.vue";

export default {
  name: "MainCompenent",
  components: {
    AboutComp,
    UpgradeSkill,
    CoursesSection,
    TestimonialSection,
    CoachSection,
    BlogSection,
  },
};
</script>

<style scoped lang="scss">
main {
  margin: 100px 0;
}
</style>