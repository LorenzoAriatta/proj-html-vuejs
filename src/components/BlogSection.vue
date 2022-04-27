<template>
  <section class="container-fluid py-5">
    <div class="la-container py-5">
      <div class="row">
        <div class="txt text-center">
          <h6>READ FOR MORE JOYMENT</h6>
          <h1>Latest From <span class="span-title">Our Blogs</span></h1>
        </div>
      </div>
      <div class="row">
        <div class="blog-card">
          <img
            class="w-100"
            src="@/assets/artist-blog-03-480x325.jpeg"
            alt="blog1"
          />
          <h6>ARTIST</h6>
          <h3>Brush Strokes Energize Trees in Painting</h3>
          <div>
            <p class="d-inline me-3">
              <i class="fa-regular fa-calendar"></i> May 15, 2020
            </p>
            <p class="d-inline"><i class="fa-regular fa-eye"></i> 688 views</p>
          </div>
        </div>
        <div class="blog-card">
          <img
            class="w-100"
            src="@/assets/artist-blog-02-480x325.jpeg"
            alt="blog2"
          />
          <h6>ARTIST</h6>
          <h3>Pocket-Sized Nootebooks Hold Miniature Paintings</h3>
          <div>
            <p class="d-inline me-3">
              <i class="fa-regular fa-calendar"></i> May 15, 2020
            </p>
            <p class="d-inline"><i class="fa-regular fa-eye"></i> 603 views</p>
          </div>
        </div>
        <div class="blog-card">
          <img
            class="w-100"
            src="@/assets/artist-blog-03-480x325.jpeg"
            alt="blog3"
          />
          <h6>ARTIST</h6>
          <h3>Connection Between Self-Portraits and Identity</h3>
          <div>
            <p class="d-inline me-3">
              <i class="fa-regular fa-calendar"></i> May 15, 2020
            </p>
            <p class="d-inline"><i class="fa-regular fa-eye"></i> 397 views</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BlogSection",
  data() {
    return {
      blogs: [
        {
          path_image: "@/assets/artist-blog-03-480x325.jpeg",
          type: "ARTIST",
          title: "Brush Strokes Energize Trees in Painting",
          date: "May 15, 2020",
          views: "688 views",
          id: 0,
        },
        {
          path_image: "@/assets/artist-blog-02-480x325.jpeg",
          type: "ARTIST",
          title: "Pocket-Sized Nootebooks Hold Miniature Paintings",
          date: "May 15, 2020",
          views: "603 views",
          id: 1,
        },
        {
          path_image: "@/assets/artist-blog-01-480x325.jpeg",
          type: "ARTIST",
          title: "Connection Between Self-Portraits and Identity",
          date: "May 15, 2020",
          views: "397 views",
          id: 2,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container-fluid {
  margin-top: 100px;
  background-color: #e2e2e0;
}
.la-container {
  width: 65%;
  margin: 0 auto;
}
h6 {
  font-weight: 500;
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
.blog-card {
  padding: 10px;
  width: calc(100% / 3 - 10px);
}
</style>