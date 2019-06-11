<template>
  <a class="btn" :class="typeButton" href="#">{{name}}</a>
</template>

<script>
  export default {
    props: ['name', 'outline'],
    computed: {
      typeButton: function() {
        return this.outline != undefined ? 'btn-outline' : 'btn-full'
      }
    }
  }
</script>

<style lang="scss" scoped>
.btn {
  &:link,
  &:visited {
    display: inline-block;
    padding: 10px 30px;
    font-weight: 300;
    text-decoration: none;
    border-radius: 200px;
    -webkit-transition: background-color 0.2s, border 0.2s, color 0.2s;
    transition: background-color 0.2s, border 0.2s, color 0.2s;
    text-transform: uppercase
  }
}

.btn-full {
  &:link,
  &:visited {
    background-color: #e67e22;
    border: 1px solid #e67e22;
    color: #fff;
    margin-right: 15px;
  }
  &:hover,
  &:active {
      background-color: #cf6d17;
  }
}

.btn-outline {
  &:link,
  &:visited {
    border: 1px solid #e67e22;
    color: #e67e22;
  }
  &:hover,
  &:active {
    border: 1px solid #cf6d17;
    color: #fff;
  }
}
</style>

