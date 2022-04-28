<template>
  <section class="la-container py-5">
    <div class="row">
      <div class="txt col-5">
        <h6>TESTIMONIALS</h6>
        <h1>Why Do People <span class="span-title">*Hearts*</span> Us?</h1>
        <p class="mb-5">
          Seeking for verbals of uor service quality? Find them here. Everything
          is transparent and straightforward for your sense of justification.
        </p>
        <p>
          <span
            ><a class="link" href="#"
              >View All <i class="fa-solid fa-arrow-right-long"></i></a
          ></span>
        </p>
      </div>
      <div class="col-7 d-flex flex-column align-items-center position">
        <TestimonialsItem
          v-for="(item, index) in people"
          :key="item.name"
          :people="people"
          :item="item"
          :index="index"
        />
      </div>
    </div>
  </section>
</template>

<script>
import TestimonialsItem from "@/components/TestimonialsItem.vue";

export default {
  name: "TestimonialSection",
  props: {
    item: Object,
  },
  components: {
    TestimonialsItem,
  },
  data() {
    return {
      people: [
        {
          image: "testimonial-01",
          name: "MADLEY PONDOR",
          work: "/ IT Specialist",
          title:
            "Professional team of specialists and passionate mentors at reach",
          review:
            "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
        },
        {
          image: "testimonial-02",
          name: "MINA HOLLACE",
          work: "/ Freelancer",
          title:
            "Professional team of specialists and passionate mentors at reach",
          review:
            "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
        },
        {
          image: "testimonial-03",
          name: "JON DOE",
          work: "/ IT Specialist",
          title:
            "Professional team of specialists and passionate mentors at reach",
          review:
            "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.la-container {
  width: 65%;
  margin: 0 auto;
}
.txt {
  padding: 60px 45px;
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
h6 {
  font-weight: 400;
  color: #6c6c6d;
}
p > span {
  margin-bottom: 5px;
  border-bottom: 1px solid #e2e2e0;
  & a {
    font-weight: 700;
    text-decoration: none;
    color: #141423;
  }
  a:hover {
    color: #1fad95;
  }
}
.position {
  position: relative;
}
</style>