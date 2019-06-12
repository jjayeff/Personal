<template>
  <nav class="container">
    <h3>{{data.logo}}</h3>
    <ul class="hidden-sm-and-down">
      <li v-for="list in data.lists" :key="list">
        <a href="#">{{list}}</a>
      </li>
    </ul>
    <i class="icon ion-md-reorder hidden-md-and-up"></i>
  </nav>
</template>

<script>
export default {
  props: ['data']
}
</script>

<style lang="scss" scoped>
  $color-underline: #e79908;
  $color-text: #fff;
  nav {
    overflow: hidden;
    padding: 1.5rem 0rem;
    h3 {
      float: left;
      text-transform: uppercase;
      letter-spacing: 0.1rem;
      padding-top: 0.7rem; 
      padding-left: 2rem; 
      color: $color-text;
    }
    ul {
      float: right;
      li {
        display: inline-block;
        padding: 1.5rem 2rem;
        a:link,
        a:visited {
          padding: 0.8rem 0;
          color: $color-text;
          text-decoration: none;
          text-transform: uppercase;
          border-bottom: 0.2rem solid transparent;
          transition: border-bottom 0.2s; 
        }
        a:hover,
        a:active {
          border-bottom: 0.2rem solid $color-underline;
        }
      }
    }

    i {
      float: right;
      font-size: 4rem;
      color: $color-text;
      padding: 0 3rem;
      cursor: pointer;
    }
  }
</style>


