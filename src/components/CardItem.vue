<template>
  <div v-if="card.value == true" class="mx-2 la-card" style="width: 24rem">
    <div class="box rounded border-0">
      <div class="img-hover-zoom">
        <img
          :src="require(`@/assets/${card.img}.jpg`)"
          class="card-img-top w-100"
          alt=""
        />
      </div>
      <div v-if="card.promotion == true" class="ribbon"><span>FREE</span></div>
    </div>
    <div class="card-body bg-white rounded">
      <h4>{{ card.price }}<span>00</span></h4>
      <h5 class="card-text mt-2 mb-5">{{ card.course }}</h5>
      <div>
        <p class="d-inline me-3">
          <i class="fa-regular fa-file"></i> {{ card.lessons }}
        </p>
        <p class="d-inline">
          <i class="fa-regular fa-user"></i> {{ card.students }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardItem",
  props: {
    card: Object,
  },
  methods: {
    // debug() {
    //   console.log(this.card);
    // },
  },
  // mounted() {
  //   this.debug();
  // },
};
</script>

<style scoped lang="scss">
h4 {
  color: #1fad95;
  font-weight: bold;
}
p {
  color: #8a9391;
  font-weight: 500;
}
span {
  font-size: 18px;
  color: #1fad95;
  font-weight: bold;
}
.card-img-top {
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}
.box {
  position: relative;
}
.ribbon {
  position: absolute;
  right: -5px;
  top: -5px;
  z-index: 1;
  overflow: hidden;
  width: 75px;
  height: 75px;
  text-align: right;
}
.ribbon span {
  font-size: 10px;
  font-weight: bold;
  color: #fff;
  text-transform: uppercase;
  text-align: center;
  line-height: 20px;
  transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  width: 100px;
  display: block;
  background: linear-gradient(#f70505 0%, #ee7455 100%);
  box-shadow: 0 3px 10px -5px rgba(0, 0, 0, 1);
  position: absolute;
  top: 19px;
  right: -21px;
}
.ribbon span::before {
  content: "";
  position: absolute;
  left: 0px;
  top: 100%;
  z-index: -1;
  border-left: 3px solid #8f0808;
  border-right: 3px solid transparent;
  border-bottom: 3px solid transparent;
  border-top: 3px solid #ee7455;
}
.ribbon span::after {
  content: "";
  position: absolute;
  right: 0px;
  top: 100%;
  z-index: -1;
  border-left: 3px solid transparent;
  border-right: 3px solid #ee7455;
  border-bottom: 3px solid transparent;
  border-top: 3px solid #8f0808;
}
.img-hover-zoom {
  height: 220px;
  overflow: hidden;
}
.img-hover-zoom img {
  transition: transform 0.5s ease;
}
.la-card:hover .img-hover-zoom img {
  transform: scale(1.5);
}
</style>