<template>
  <div class="la-container py-5">
    <div class="row">
      <div class="txt col-5">
        <h6>EVERYTHING IN <strong class="fw-bold">MAXCOACH</strong></h6>
        <h1>
          Learn about our <span class="span-title">Work Culture</span> at
          MaxCoach
        </h1>
        <p class="mb-5">
          Spend some time to visit our website or head office and discover our
          current courses, enrollment precedure, and registration deadline.
          We're opening new classes every beginning of each month.
        </p>
        <p>
          Have questions?
          <span
            ><a class="link" href="#"
              >Get Free Guide <i class="fa-solid fa-arrow-right-long"></i></a
          ></span>
        </p>
        <div class="circle"></div>
        <div class="grid">
          <img src="@/assets/maxcoach-shape-07-150x150.png" alt="#" />
        </div>
      </div>
      <div class="content col-7 d-flex justify-content-end">
        <img
          class="rounded"
          style="height: 450px"
          src="@/assets/stock-full-hd-10.jpg"
          alt="#"
        />
        <div class="img-desi">
          <img
            class="rounded img-about"
            src="@/assets/about-us-01.jpg"
            alt="#"
          />
        </div>
        <div class="round-shape">
          <img src="@/assets/maxcoach-shape-02.png" alt="#" />
        </div>
      </div>
    </div>
    <div class="row justify-content-center data">
      <div class="col-3 text-center">
        <h1>129+</h1>
        <h6>ENROLLED LEARNERS</h6>
      </div>
      <div class="col-3 text-center">
        <h1>80</h1>
        <h6>FINISHED SESSIONS</h6>
      </div>
      <div class="col-3 text-center">
        <h1>4%</h1>
        <h6>SATISFACTION RATE</h6>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutComp",
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
}
.txt {
  position: relative;
  padding: 60px 45px;
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
    a:hover {
      color: #1fad95;
    }
  }
}
.content {
  position: relative;
}
.img-desi {
  position: absolute;
  bottom: 72%;
  left: 83%;
}
.grid {
  position: absolute;
  left: 205%;
  bottom: 80%;
}
.round-shape {
  position: absolute;
  left: 70%;
  top: 77%;
}
.data {
  margin: 50px 0px;
  & h1 {
    color: #1fad95;
    font-weight: 700;
  }
  & h6 {
    font-weight: bold;
  }
}
</style>