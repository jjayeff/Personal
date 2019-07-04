<template>
  <section class="portfolio">
    <div class="container">
      <h2>Portfolio</h2>
      <div class="row">
        <div class="col-md-3 col-xs-6" v-for="list in lists" :key="list.name">
          <img :src="list.img" alt="Lisbon">
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
            name: 'Project1',
            img: 'https://s.isanook.com/ca/0/ud/279/1395449/56480274_2523567494381821_363.jpg'
          },
          {
            name: 'Project2',
            img: 'https://hilight.kapook.com/img_cms2/user/surauch/news/pareena.jpg'
          },
          {
            name: 'Project3',
            img: 'https://static.wixstatic.com/media/55a97f_74f94a7240c044a78c59eb3f378c240e~mv2.jpg/v1/fill/w_303,h_303,al_c,lg_1,q_80/55a97f_74f94a7240c044a78c59eb3f378c240e~mv2.jpg'
          },
          {
            name: 'Project4',
            img: 'https://pbs.twimg.com/media/D8RFAQsWsAclw0E.jpg'
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  .portfolio {
    background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),url(../../assets/img/park-2693078_1920.jpg);
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
