<template>
  <nav class="container">
    <h1>{{data.logo}}</h1>
    <ul>
      <li v-for="list in data.lists" :key="list">
        <a href="#">{{list}}</a>
      </li>
    </ul>
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
    padding-top: 15px;
    padding-bottom: 15px;
    h1 {
      float: left;
      text-transform: uppercase;
      font-weight: 300;
      letter-spacing: 1px;
      padding-top: 2px; 
      padding-left: 20px; 
      color: $color-text;
    }
    ul {
      float: right;
      li {
        display: inline-block;
        padding: 10px 20px;
        a:link,
        a:visited {
          padding: 8px 0;
          color: $color-text;
          text-decoration: none;
          text-transform: uppercase;
          font-size: 90%;
          border-bottom: 2px solid transparent;
          transition: border-bottom 0.2s; 
        }
        a:hover,
        a:active {
          border-bottom: 2px solid $color-underline;
        }
      }
    }
  }
</style>


