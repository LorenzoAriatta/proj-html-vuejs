<template>
  <div
    class="row card-testimonial"
    @click="changeCard(index)"
    :class="selectedCard(index)"
  >
    <div class="col-12">
      <h5>{{ item.title }}</h5>
      <h6>{{ item.review }}</h6>
    </div>
    <div class="row">
      <div class="col-3">
        <img
          class="rounded-circle"
          :src="require(`@/assets/${item.image}.jpg`)"
          :alt="item.name"
        />
      </div>
      <div class="col-9">
        <h6>{{ item.name }}</h6>
        <p>{{ item.work }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TestimonialsItem",
  data() {
    return {
      indexSelected: 0,
    };
  },
  props: {
    index: Number,
    item: Object,
    people: Array,
  },
  mounted() {
    //this.debug();
  },
  methods: {
    debug() {
      console.log(this.index);
    },
    changeCard(index) {
      if (this.indexSelected !== index) {
        this.indexSelected = index;
      }
    },
    selectedCard(index) {
      if (this.indexSelected === index) {
        return "absolute-center";
      } else if (this.indexSelected !== index) {
        return "default-position";
      }
    },
  },
};
</script>

<style scoped lang="scss">
.card-testimonial {
  padding: 20px;
}
img {
  width: 80px;
  height: 80px;
}
.absolute-center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 2000;
  background-color: white;
  border: 2px solid black;
  width: 650px;
  height: 300px;
}
.default-position {
  background-color: white;
  border: 2px solid black;
  width: 500px;
  height: 250px;
  margin: 20px 0;
  opacity: 50%;
}
</style>