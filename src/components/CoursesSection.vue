<template>
  <section id="svg-shape" class="container-fluid py-5">
    <div class="la-container row flex-column align-items-center">
      <div class="txt text-center col-6">
        <h6>JOIN MAXCOACH AT BEST</h6>
        <h1>Latest Online <span class="span-title">Courses</span></h1>
      </div>
      <SliderCards />
      <div id="link" class="col-6 text-center mt-5">
        <h5>
          Control your personal preference settings to get notified about
          appropriate courses.
          <span
            ><a href="#"
              >View all courses <i class="fa-solid fa-arrow-right-long"></i></a
          ></span>
        </h5>
      </div>
    </div>
    <svg
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 100 100"
      preserveAspectRatio="none"
      height="100"
    >
      <path class="elementor-shape-fill" d="M0 0v100h100V0Q50 200 0 0" />
    </svg>
  </section>
</template>

<script>
import SliderCards from "@/components/SliderCards.vue";

export default {
  components: {
    SliderCards,
  },
  name: "CoursesSection",
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
}
#svg-shape {
  position: relative;
}
svg {
  position: absolute;
  width: 100%;
  top: 89.6%;
  right: 0%;
  filter: invert(1);
}
.container-fluid {
  background: linear-gradient(#ffffff, #e2e2e0);
  background-repeat: no-repeat;
}
h6,
h5 {
  font-weight: 400;
  color: #6c6c6d;
  & span {
    margin-bottom: 5px;
    border-bottom: 1px solid #e2e2e0;
    & a {
      font-weight: 700;
      text-decoration: none;
      color: #141423;
    }
    a:hover {
      color: #1fad95;
    }
  }
}
h1 {
  color: #22272d;
  font-size: 52px;
  font-weight: 700;
  & .span-title {
    color: #1fad95;
    font-weight: 300;
  }
}
#link {
  margin-bottom: 45px;
}
.txt {
  position: relative;
  padding: 60px 45px;
}
.shape {
  position: absolute;
}
</style>