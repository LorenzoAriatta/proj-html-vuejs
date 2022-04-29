<template>
  <div
    class="row card-testimonial justify-content-around"
    @click="activate(item.id)"
    :class="isActive === item.id ? 'absolute-center' : 'default-position'"
  >
    <div class="col-12 mt-2">
      <h5>{{ item.title }}</h5>
      <h6 class="mt-3">{{ item.review }}</h6>
    </div>
    <div class="row align-items-center">
      <div class="col-2">
        <img
          class="rounded-circle"
          :src="require(`@/assets/${item.image}.jpg`)"
          :alt="item.name"
        />
      </div>
      <div class="col-10">
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
      isActive: 0,
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
    activate(id) {
      this.isActive = id;
      let selected = document.querySelector(".absolute-center");
      selected.classList.remove("absolute-center");
      selected.classList.add("default-position");
    },
    selectedCard(index) {
      if (
        this.indexSelected === 0 &&
        this.indexSelected !== 1 &&
        this.indexSelected !== 2
      ) {
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
  box-shadow: 13px 0px 60px -15px grey;
}
.default-position:hover {
  transition: 0.4s;
  transform: scale(0.9);
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
  width: 630px;
  height: 300px;
}
.default-position {
  background-color: white;
  width: 550px;
  height: 250px;
  margin: 20px 0;
  opacity: 50%;
}
</style>