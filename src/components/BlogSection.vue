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
        <div v-for="blog in blogs" :key="blog.id" class="blog-card">
          <img
            class="w-100 rounded mb-3"
            :src="require(`@/assets/${blog.image}.jpg`)"
            :alt="blog.title"
          />
          <h6>{{ blog.type }}</h6>
          <h3 class="mb-3">{{ blog.title }}</h3>
          <div>
            <p class="d-inline me-3">
              <i class="fa-regular fa-calendar"></i> {{ blog.date }}
            </p>
            <p class="d-inline">
              <i class="fa-regular fa-eye"></i> {{ blog.views }}
            </p>
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
          image: "blog-03",
          type: "ARTIST",
          title: "Brush Strokes Energize Trees in Painting",
          date: "May 15, 2020",
          views: "688 views",
          id: 0,
        },
        {
          image: "blog-01",
          type: "ARTIST",
          title: "Pocket-Sized Nootebooks Hold Miniature Paintings",
          date: "May 15, 2020",
          views: "603 views",
          id: 1,
        },
        {
          image: "blog-02",
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