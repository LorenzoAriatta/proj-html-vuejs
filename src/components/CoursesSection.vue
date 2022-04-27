<template>
  <section class="container-fluid py-5">
    <div class="la-container row flex-column align-items-center">
      <div class="txt text-center col-6">
        <h6>JOIN MAXCOACH AT BEST</h6>
        <h1>Latest Online <span class="span-title">Courses</span></h1>
      </div>
      <div class="col-6 text-center">
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
  </section>
</template>

<script>
export default {
  name: "CoursesSection",
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
}
// .container-fluid {
//   background-image: url(@/assets/svg-1.svg);
//   background-repeat: no-repeat;
// }
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
.txt {
  position: relative;
  padding: 60px 45px;
}
.shape {
  position: absolute;
}
</style>