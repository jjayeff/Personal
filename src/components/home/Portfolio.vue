<template>
  <section class="portfolio">
    <div class="container">
      <h2>Portfolio</h2>
      <div class="row">
        <div class="col-md-4 col-xs-12" v-for="list in lists" :key="list.name" :onclick="list.link">
          <img :src="list.img" alt="Lisbon" />
          <h3>{{list.name}}</h3>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      lists: [
        {
          name: "Ekkawit",
          img: require("../../assets/img/personal.png"),
          link: "window.open('https://ekkawitl.netlify.com/','new_window');"
        },
        {
          name: "FindStock",
          img: require("../../assets/img/FindStock2.png"),
          link:
            "window.open('https://findstock-core.netlify.com/','new_window');"
        },
        {
          name: "Luss-Official",
          img: require("../../assets/img/luss.png"),
          link:
            "window.open('https://luss-official.netlify.com/','new_window');"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.portfolio {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(../../assets/img/park-2693078_1920.jpg);
  background-size: cover;
  background-attachment: fixed;
  padding: 50px;
  color: #fff;
  text-align: center;

  img {
    cursor: pointer;
    width: 80%;
    height: auto;
  }

  h3 {
    font-size: 130%;
    margin: 10px 0px;
    font-weight: 300;
    text-transform: uppercase;
    letter-spacing: 1px;
    cursor: pointer;
  }

  h2 {
    font-size: 180%;
    word-spacing: 2px;
    margin-bottom: 30px;
    letter-spacing: 1px;
    text-align: center;
    font-weight: 300;
    text-transform: uppercase;
    &:after {
      display: block;
      height: 2px;
      background-color: #e97e22;
      content: "";
      width: 100px;
      margin: 0 auto;
      margin-top: 20px;
    }
  }

  .row {
    margin-top: 50px;
  }
}
</style>
