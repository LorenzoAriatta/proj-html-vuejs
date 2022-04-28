<template>
  <div class="la-container">
    <div class="row flex-nowrap justify-content-center">
      <CardItem
        v-for="card in cards"
        :key="card.id"
        :card="card"
        :cards="cards"
      />
    </div>
    <div class="row btn-slide mt-5">
      <div>
        <div class="dot"></div>
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
  data() {
    return {
      cards: [
        {
          img: "course-04",
          price: "$60.",
          course: "Introduction to Cybersecurity",
          lessons: "21 Lessons",
          students: "520 Students",
          id: 5,
          value: false,
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
          course: "Data Analysis: Computer Simulation",
          lessons: "28 Lessons",
          students: "389 Students",
          id: 4,
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
}
.btn-slide {
  text-align: -webkit-center;
}
</style>