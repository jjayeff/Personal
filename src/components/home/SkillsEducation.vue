<template>
  <section class="skills-education">
    <div class="container">
      <div class="skill">
        <h3>my skill</h3>
        <div class="row">
          <div class="col-lg-6">
            <h5>programing</h5>
            <ul class="row">
              <li class="col-xs-6 col-sm-4" v-for="skill in skills" :key="skill.name">
                <span>{{skill.name}}</span>
                <img :src="skill.img" alt="">
              </li>
            </ul>
          </div>
          <div class="col-lg-6">
            <h5>experience with</h5>
            <ul class="row border-left">
              <li class="col-xs-6 col-sm-4 col-md-6 " v-for="experience in experiences" :key="experience.name">
                <span>{{experience.name}}</span>
                <img :src="experience.img" alt="">
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        skills: [
          {
            name: 'HTML5',
            img: require('../../assets/img/html5.png')
          },
          {
            name: 'CSS3',
            img: require('../../assets/img/css3.svg')
          },
          {
            name: 'Javascript',
            img: require('../../assets/img/js.png')
          },
          {
            name: 'JQuery',
            img: require('../../assets/img/jq.gif')
          },
          {
            name: 'C++',
            img: require('../../assets/img/c++.png')
          },
          {
            name: 'C#/ASP.net',
            img: require('../../assets/img/cship.png')
          },
          {
            name: 'JAVA',
            img: require('../../assets/img/java.png')
          },
          {
            name: 'PHP',
            img: require('../../assets/img/php.png')
          },
          {
            name: 'MySQL',
            img: require('../../assets/img/mysql.png')
          }
        ],
        experiences: [
          {
            name: 'Node js',
            img: require('../../assets/img/node.jpg')
          },
          {
            name: 'React/Redux',
            img: require('../../assets/img/react.png')
          },
          {
            name: 'Next js',
            img: require('../../assets/img/next.png')
          },
          {
            name: 'React Native',
            img: require('../../assets/img/react-native.png')
          },
          {
            name: 'Vue/Vuex',
            img: require('../../assets/img/vue.png')
          },
          {
            name: 'Nosql',
            img: require('../../assets/img/nosql.png')
          }
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  .skills-education {
    margin: 5rem;
  }
  .skill {
    margin-bottom: 10rem;
    text-align: center;
    h3 {
      word-spacing: 0.2rem;
      margin-bottom: 3rem;
      letter-spacing: 0.1rem;
      font-weight: 300;
      text-transform: uppercase;
      &:after {
        display: block;
        height: 0.2rem;
        background-color: #e97e22;
        content: "";
        width: 10rem;
        margin: 0 auto;
        margin-top: 2rem;
      }
    }
    h5 {
      word-spacing: 0.2rem;
      margin-bottom: 3rem;
      letter-spacing: 0.1rem;
      font-weight: 300;
      text-transform: uppercase;
      &:after {
        display: block;
        height: 0.2rem;
        background-color: #e97e22;
        content: "";
        width: 10rem;
        margin: 0 auto;
        margin-top: 0.5rem;
      }
    }

    .border-left {
      border-left: 0.2rem solid #e97e22;
    }

    li {
      padding: 0.5rem;

      img {
        height: 3rem;
        width: auto;
        vertical-align: middle; /* | top | bottom */
        margin-left: 2rem;
      }

      span {
        display: inline-block;
        vertical-align: middle; /* | top | bottom */
      }
    }
  }

  @media only screen and (max-width: 992px) {
    .skill {
      .border-left {
        border-left: transparent;
      }
    }
  }
</style>

