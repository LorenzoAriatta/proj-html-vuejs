<template>
  <section class="py-5">
    <div class="la-container">
      <div class="txt row flex-column align-items-center">
        <div class="shape-circle">
          <img src="@/assets/maxcoach-shape-02.png" alt="#" />
        </div>
        <div class="grid">
          <img src="@/assets/maxcoach-shape-09.png" alt="" />
        </div>
        <div class="txt text-center col-6">
          <h1>Subscribe <span class="span-title">Newsletters</span></h1>
        </div>
        <div class="col-6 text-center mt-3">
          <h5>
            Enter your email address to register to our newsletter subscription
            delivered on a regular basis!
          </h5>
        </div>
      </div>
      <div class="row flex-wrap justify-content-center mt-5 anchor">
        <input class="col-5" type="text" placeholder=" Enter your email" />
        <button class="col-2 la-button" type="submit">Subscribe</button>
        <div class="circle"></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SubscribeSection",
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
}
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
input {
  border: none;
  background-color: #e2e2e0;
  color: #6c6c6d;
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
}
.la-button {
  background-color: #1fad95;
  color: white;
  border: none;
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
  font-size: 13px;
  font-weight: bolder;
  padding: 15px 0px;
}
.la-button:hover {
  transition: 0.3s;
  background-color: #198575;
}
.anchor {
  position: relative;
}
.txt {
  position: relative;
}
.circle {
  position: absolute;
  right: 100%;
  top: -45%;
  height: 60px;
  width: 60px;
  background-color: white;
  border-radius: 50%;
  border: 7px solid #1fad95;
  filter: opacity(60%);
}
.shape-circle {
  position: absolute;
  left: 90%;
  width: 127px;
  top: 65%;
}
.grid {
  position: absolute;
  left: 85%;
  width: 204px;
  top: 0%;
}
</style>