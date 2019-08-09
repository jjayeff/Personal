<template>
  <section class="experience">
    <div class="container">
      <h3>Experience</h3>
      <app-timeline :data="lists" />
    </div>
  </section>
</template>

<script>
import appTimeline from "../core/Timeline1.vue";
export default {
  components: {
    appTimeline
  },
  data() {
    return {
      lists: [
        {
          pointion: "Intership",
          company: "ITTP",
          info: "React, React Native, MongoDB",
          start: "MAY, 2017",
          end: "DEC, 2017"
        },
        {
          pointion: "Programmer",
          company: "Toptrader",
          info: "C++, C#/ASP.net, MySQL",
          start: "JUNE, 2018",
          end: "MAY, 2019"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.experience {
  background-color: #f4f4f4;
  padding: 5rem;
  h3 {
    word-spacing: 0.2rem;
    letter-spacing: 0.1rem;
    text-align: center;
    font-weight: 300;
    text-transform: uppercase;
    &:after {
      display: block;
      height: 0.1rem;
      background-color: #e97e22;
      content: "";
      width: 10rem;
      margin: 0 auto;
      margin-top: 2rem;
    }
  }
}
</style>
