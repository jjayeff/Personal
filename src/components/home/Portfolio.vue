<template>
  <section class="portfolio">
    <div class="container">
      <h2>Portfolio</h2>
      <div class="row">
        <div class="col span-1-of-4 box" v-for="list in lists" :key="list.name">
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
            name: 'FindStock',
            img: 'https://s.isanook.com/ca/0/ud/279/1395449/56480274_2523567494381821_363.jpg'
          },
          {
            name: 'FindStock',
            img: 'https://hilight.kapook.com/img_cms2/user/surauch/news/pareena.jpg'
          },
          {
            name: 'FindStock',
            img: 'https://static.wixstatic.com/media/55a97f_74f94a7240c044a78c59eb3f378c240e~mv2.jpg/v1/fill/w_303,h_303,al_c,lg_1,q_80/55a97f_74f94a7240c044a78c59eb3f378c240e~mv2.jpg'
          },
          {
            name: 'FindStock',
            img: 'https://pbs.twimg.com/media/D8RFAQsWsAclw0E.jpg'
          },
          {
            name: 'FindStock',
            img: 'https://site-assets.mediaoxide.com/workpointnews/2018/06/21161010/1529572207_41633_chuwit.png'
          },
          {
            name: 'FindStock',
            img: 'https://scontent-fbkk5-7.us-fbcdn.net/v1/t.1-48/1426l78O9684I4108ZPH0J4S8_842023153_K1DlXQOI5DHP/dskvvc.qpjhg.xmwo/w/data/1133/1133409-img.tjmuhy.0p.jpg'
          },
          {
            name: 'FindStock',
            img: 'https://hilight.kapook.com/img_cms2/user/amusic/a3_184.jpg'
          }
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
      width: 90%;
      height: 240px;
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
