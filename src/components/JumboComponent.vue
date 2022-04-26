<template>
  <div class="container-fluid text-center">
    <div class="tools d-flex flex-column">
      <div>
        <a href="#"><i class="fa-regular fa-bookmark"></i></a>
      </div>
      <div class="my-2">
        <a href="#"><i class="fa-regular fa-life-ring"></i></a>
      </div>
      <div class="mb-2">
        <a href="#"><i class="fa-solid fa-book"></i></a>
      </div>
      <div>
        <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
      </div>
    </div>
    <div class="content">
      <div class="text-white">
        <h2>Commence Business</h2>
        <h1>Distant Mentoring Program</h1>
      </div>
      <button class="la-button mt-4" type="submit">
        Download free guidebook <i class="fa-solid fa-arrow-right-long"></i>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumboComponent",
};
</script>

<style scoped lang="scss">
.container-fluid {
  background-image: url(@/assets/home-3-hero-bg.jpg);
  background-repeat: no-repeat;
  position: relative;
  padding: 50px 0;
}
.tools {
  position: absolute;
  top: 20%;
  left: 97.4%;
  padding: 10px 15px;
  background-color: #fff;
  & a {
    color: black;
    font-size: 18px;
    & :hover {
      color: #1fad95;
    }
  }
}
.content {
  margin: 190px auto;
}
h2 {
  font-weight: bold;
}
h1 {
  font-size: 70px;
  font-weight: lighter;
}
.la-button {
  background-color: white;
  color: #1fad95;
  border: none;
  border-radius: 5px;
  font-size: 13px;
  font-weight: bolder;
  padding: 15px 40px;
}
.la-button:hover {
  transition: 0.3s;
  background-color: #1fad95;
  color: white;
}
</style>