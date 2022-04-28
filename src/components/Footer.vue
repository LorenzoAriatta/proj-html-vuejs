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
          <div class="d-flex flex-row">
            <div class="col-4 d-flex flex-column flex-wrap">
              <ul>
                <h5>Explore</h5>
                <li v-for="(link, index) in exploreLinks" :key="link.index">
                  <a href="#">{{ exploreLinks[index] }}</a>
                </li>
              </ul>
            </div>
            <div class="col-8">
              <ul>
                <h5>Information</h5>
                <li v-for="(link, index) in informationLinks" :key="link.index">
                  <a href="#">{{ informationLinks[index] }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComp",
  data() {
    return {
      exploreLinks: [
        "Start here",
        "Blog",
        "About us",
        "Sussess story",
        "Courses",
        "Contact us",
      ],
      informationLinks: [
        "Membership",
        "Purchase guide",
        "Privacy policy",
        "Terms of service",
      ],
    };
  },
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
.icon a {
  color: #b1b1b0;
  font-size: 35px;
  & i:hover {
    color: #1fad95;
    transform: scale(1.1);
  }
}
li {
  list-style-type: none;
  & a {
    color: #b1b1b0;
    text-decoration: none;
  }
  & a:hover {
    color: #1fad95;
    font-weight: 400;
  }
}
</style>