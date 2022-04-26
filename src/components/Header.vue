<template>
  <div class="container-fluid py-4">
    <div class="la-container">
      <div class="row align-items-center justify-content-around">
        <div class="col-5 d-flex">
          <nav>
            <ul>
              <li>
                <a href="#">Home</a>
              </li>
              <li>
                <a href="#">Pages</a>
              </li>
              <li>
                <a href="#">Courses</a>
              </li>
              <li>
                <a href="#">Features</a>
              </li>
              <li>
                <a href="#">Blog</a>
              </li>
              <li>
                <a href="#">Shop</a>
              </li>
            </ul>
          </nav>
        </div>
        <div class="col-2 d-flex">
          <div class="logo">
            <img src="@/assets/dark-logo.png" alt="logo" class="w-100" />
          </div>
        </div>
        <div class="col-5 d-flex justify-content-end">
          <div class="icons d-flex align-items-center">
            <div class="cart me-4">
              <i class="fa-solid fa-cart-shopping"></i>
              <span
                class="
                  alert
                  top-0
                  start-100
                  translate-middle
                  badge
                  border border-light
                  rounded-circle
                  p-2
                "
                >0</span
              >
            </div>
            <div class="user me-4">
              <i class="fa-regular fa-circle-user"></i>
            </div>
            <div class="search-wrapper">
              <input type="text" placeholder="  Search..." />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {},
};
</script>

<style scoped lang="scss">
.la-container {
  width: 80%;
  margin: 0 auto;
}
ul {
  margin: 0%;
}
li {
  list-style-type: none;
  display: inline;
  margin-right: 2rem;
  & a {
    text-decoration: none;
    color: #22272d;
    font-weight: 500;
  }
}
li:after {
  font-family: "FontAwesome";
  content: "\f078";
  color: #22272d;
  font-size: 8px;
  margin-left: 5px;
}
.search-wrapper {
  display: inline-block;
  position: relative;
  & input {
    background-color: #e1e1e1;
    border: none;
    border-radius: 5px;
    padding: 5px;
  }
}
.search-wrapper::after {
  font-family: "FontAwesome";
  content: "\f002";
  color: #1fad95;
  position: absolute;
  right: 6px;
  top: 6px;
}
.cart {
  position: relative;
  font-size: 18px;
}
.user {
  font-size: 18px;
}
.alert {
  position: absolute;
  background-color: #1fad95;
  font-size: 12px;
  text-align: center;
  line-height: 1px;
  width: 4px;
}
</style>
