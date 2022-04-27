<template>
  <footer class="container-fluid py-5">
    <div class="la-container">
      <div class="row">
        <div class="col-6">
          <h5>Address</h5>
          <p>382 NE 191st St # Miami, FL 33179-3899</p>
          <p>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
          <p>support@maxcoach.com</p>
          <div class="social">
            <div class="icon d-inline me-4">
              <a href="#"><i class="fa-brands fa-twitter"></i></a>
            </div>
            <div class="icon d-inline me-4">
              <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
            </div>
            <div class="icon d-inline me-4">
              <a href="#"><i class="fa-brands fa-instagram"></i></a>
            </div>
            <div class="icon d-inline me-4">
              <a href="#"><i class="fa-brands fa-linkedin"></i></a>
            </div>
          </div>
        </div>
        <div class="col-6 links">
          <div class="explore d-flex flex-column flex-wrap">
            <ul>
              <h5>Explore</h5>
              <li><a href="#">Star here</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">About Us</a></li>
              <li><a href="#">Success story</a></li>
              <li><a href="#">Courses</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComp",
};
</script>

<style scoped lang="scss">
footer {
  background-color: #141423;
}
.la-container {
  width: 65%;
  margin: 0 auto;
}
h5 {
  color: white;
}
p {
  color: #b1b1b0;
  font-size: 14px;
}
a {
  color: #b1b1b0;
  font-size: 26px;
}
li {
  list-style-type: none;
  & a {
    text-decoration: none;
  }
}
</style>