<template>
  <section class="skills-education">
    <div class="container">
      <div class="skill">
        <h2>my skill</h2>
        <div class="row">
          <div class="col span-1-of-2">
            <h3>programing</h3>
            <ul class="row">
              <li class="col span-1-of-3" v-for="skill in skills" :key="skill.name">
                <span>{{skill.name}}</span>
                <img :src="skill.img" alt="">
              </li>
            </ul>
          </div>
          <div class="col span-1-of-2">
            <h3>experience with</h3>
            <ul class="row border-left">
              <li class="col span-1-of-2" v-for="experience in experiences" :key="experience.name">
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
    margin: 50px;
  }
  .skill {
    margin-bottom: 100px;
    text-align: center;
    h2 {
      font-size: 180%;
      word-spacing: 2px;
      margin-bottom: 30px;
      letter-spacing: 1px;
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
    h3 {
      text-align: center;
      text-transform: uppercase;
      margin-bottom: 20px;
      &:after {
        display: block;
        height: 2px;
        background-color: #e97e22;
        content: "";
        width: 100px;
        margin: 0 auto;
        margin-top: 5px;
      }
    }

    .border-left {
      border-left: 2px solid #e97e22;
    }

    li {
      padding: 5px;

      img {
        height: 30px;
        width: auto;
        vertical-align: middle; /* | top | bottom */
        margin-left: 20px;
      }

      span {
        display: inline-block;
        vertical-align: middle; /* | top | bottom */
      }
    }
  }
</style>

