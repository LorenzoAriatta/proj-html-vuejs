<template>
  <section class="la-container py-5">
    <div class="grid-circle">
      <img src="@/assets/maxcoach-shape-05.png" alt="#" />
    </div>
    <div class="shape">
      <svg xmlns="http://www.w3.org/2000/svg" width="200" height="202">
        <path
          class="elementor-shape-fill"
          d="M139.374 198.088c16.328 8.906 51.35-1.087 58.304-39.038 7.15-39.022-13.182-40.052-9.633-54.248 14.243-21.15 16.782-48.14 2.028-64.387-36.503-38.024-45.629 7.604-76.048-20.28C101.727 7.837 83.1-6.735 56.23 3.405 18.239 17.74 27.33 47.659 27.33 69.313c0 7.624-24.216 21.957-26.87 41.573-3.346 24.734 12.168 57.29 26.87 68.443 23.322 26.363 59.318 20.28 75.541 11.154 13.931-7.836 25.35 1.52 36.503 7.605z"
        />
      </svg>
    </div>
    <div class="grid">
      <img src="@/assets/maxcoach-shape-07.png" alt="#" />
    </div>
    <div class="row">
      <div class="col-7 d-flex justify-content-center content">
        <img class="rounded" src="@/assets/home-3-team-image.png" alt="#" />
        <div class="shape-lines">
          <img src="@/assets/maxcoach-shape-01.png" alt="#" />
        </div>
      </div>
      <div class="txt col-5">
        <h6>EVERYTHING IN <strong class="fw-bold">MAXCOACH</strong></h6>
        <h1>We're Here To <span class="span-title">Transform</span> You!</h1>
        <p class="mb-5">
          As learners, people can enjoy great companionship from MaxCoach
          mentors and educators. We can help you develop and grow at your best.
        </p>
        <button class="la-button" type="submit">Get Free Guide</button>
        <div class="circle"></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "CoachSection",
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
  position: relative;
}
h6 {
  font-weight: 400;
  color: #6c6c6d;
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
.la-button {
  background-color: #1fad95;
  color: white;
  border: none;
  border-radius: 5px;
  font-size: 13px;
  font-weight: bolder;
  padding: 20px 60px;
}
.la-button:hover {
  transition: 0.3s;
  background-color: #198575;
}
.circle {
  position: absolute;
  bottom: 97%;
  right: 90%;
  height: 60px;
  width: 60px;
  background-color: white;
  border-radius: 50%;
  border: 7px solid #ecc5ab;
}
.content {
  position: relative;
}
.shape-lines {
  position: absolute;
  top: 90%;
  right: 100%;
}
.grid-circle {
  position: absolute;
  right: 87%;
  top: 30%;
}
.shape {
  fill: #1fad95;
  position: absolute;
  bottom: 50%;
  right: 80%;
}
svg {
  filter: opacity(50%);
  transform: scale(0.8);
}
.grid {
  position: absolute;
  top: 80%;
  left: 25%;
}
</style>