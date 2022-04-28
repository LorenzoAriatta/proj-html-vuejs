<template>
  <div class="la-container">
    <div class="row flex-nowrap justify-content-center wrapp-card">
      <CardItem
        v-for="(card, index) in cards"
        :key="index"
        :card="card"
        :cards="cards"
        :index="index"
        :min="min"
        :max="max"
      />
    </div>
    <div class="row btn-slide mt-5">
      <div>
        <button
          @click="slideCard(0, 2)"
          :class="selectedBtn(0)"
          class="dot me-3"
        ></button>
        <button
          @click="slideCard(1, 3)"
          :class="selectedBtn(1)"
          class="dot me-3"
        ></button>
        <button
          @click="slideCard(2, 4)"
          :class="selectedBtn(2)"
          class="dot me-3"
        ></button>
        <button
          @click="slideCard(3, 5)"
          :class="selectedBtn(3)"
          class="dot me-3"
        ></button>
        <button
          @click="slideCard(4, 6)"
          :class="selectedBtn(4)"
          class="dot me-3"
        ></button>
      </div>
    </div>
  </div>
</template>

<script>
import CardItem from "@/components/CardItem.vue";
export default {
  components: {
    CardItem,
  },
  name: "SliderCards",
  methods: {
    selectedBtn(num) {
      if (this.min === num) {
        return "active";
      }
      return "dot";
    },
    slideCard(a, b) {
      this.min = a;
      this.max = b;
    },
    autoPlay() {
      const timer = setInterval(() => {
        this.min++;
        this.max++;
        if (this.max >= 6 && this.min >= 4) {
          this.max = 2;
          this.min = 0;
        }
      }, 8000);
      console.log(this.min, this.max, timer);
    },
  },
  mounted() {
    this.autoPlay();
  },
  data() {
    return {
      min: 0,
      max: 2,
      cards: [
        {
          img: "course-01",
          price: "$40.",
          course: "Learning to Write as a Professional Author",
          lessons: "20 Lessons",
          students: "50 Students",
          id: 0,
          value: true,
        },
        {
          img: "course-02",
          price: "$0.",
          course: "Customer-centric Info-Tech Strategies",
          lessons: "24 Lessons",
          students: "769 Students",
          id: 1,
          value: true,
          promotion: true,
        },
        {
          img: "course-03",
          price: "$19.",
          course: "Open Programming Courses for Everyone: Phyton",
          lessons: "17 Lessons",
          students: "62 Students",
          id: 2,
          value: true,
        },
        {
          img: "course-04",
          price: "$80.",
          course: "Communication: Business Writing and Storytelling",
          lessons: "32 Lessons",
          students: "154 Students",
          id: 3,
          value: false,
        },
        {
          img: "course-05",
          price: "$180.",
          course: "Certificate in Data Analysis: Computer Simulation",
          lessons: "28 Lessons",
          students: "389 Students",
          id: 4,
          value: false,
        },
        {
          img: "course-04",
          price: "$0.",
          course: "Introduction to Cybersecurity: Beginner to Intermediate",
          lessons: "21 Lessons",
          students: "520 Students",
          id: 5,
          value: false,
          promotion: true,
        },
        {
          img: "course-03",
          price: "$520.",
          course: "Postgraduate Certificate in Data Analytics",
          lessons: "42 Lessons",
          students: "48 Students",
          id: 6,
          value: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.dot {
  width: 8px;
  height: 8px;
  background-color: #b1b1b0;
  border-radius: 50%;
  border: none;
}
.btn-slide .dot:hover {
  transition: 0.3s;
  transform: scale(2);
  background-color: #1fad95;
}
.active {
  transform: scale(2);
  background-color: #1fad95;
}
.btn-slide {
  text-align: -webkit-center;
}
</style>