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
      <div class="col-7 content">
        <img
          class="rounded"
          src="@/assets/stock-full-hd-11-670x450.jpg"
          alt="#"
        />
        <div class="youtube">
          <img src="@/assets/icon-youtube-play.png" alt="#" />
        </div>
      </div>
      <div class="txt col-5">
        <h6>HOW WE WORK</h6>
        <h1>
          Upgrade Your Skills <span class="span-title">Upgrade Your Life</span>
        </h1>
        <p class="mb-5">
          Opening up more opportunities in front of you to get the ticket to
          more enjoyable door in life. Getting equipped with new skills for new
          sets of insights into your career. MaxCoach accompany learners in
          every stage of learning.
        </p>
        <p>
          <span
            ><a class="link" href="#"
              >Download free guidebook
              <i class="fa-solid fa-arrow-right-long"></i></a
          ></span>
        </p>
        <div class="circle"></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "UpgradeSkill",
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
p {
  & span {
    margin-bottom: 10px;
    border-bottom: 1px solid #e2e2e0;
    & a {
      color: #141423;
      text-decoration: none;
      font-weight: bold;
    }
  }
}
.txt {
  position: relative;
  padding: 60px 45px;
}
.circle {
  position: absolute;
  bottom: 95%;
  left: 8%;
  height: 60px;
  width: 60px;
  background-color: white;
  border-radius: 50%;
  border: 7px solid #ecc5ab;
}
.content {
  position: relative;
  & > img {
    box-shadow: 30px 30px 135px -50px #6c6c6d;
  }
}
.youtube {
  position: absolute;
  top: 36%;
  left: 41%;
}
.grid-circle {
  position: absolute;
  right: 94%;
  top: 15%;
}
.shape {
  position: absolute;
  bottom: 75%;
  right: 90%;
}
svg {
  filter: opacity(10%);
  transform: scale(0.8);
}
.grid {
  position: absolute;
  top: 70%;
  left: 42%;
}
</style>