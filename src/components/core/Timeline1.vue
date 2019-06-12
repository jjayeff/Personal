<template>
  <div class="box">
    <ul id="first-list">
      <li v-for="list in data" :key="list.company">
        <span></span>
        <div class="title">{{list.pointion}}</div>
        <div class="text-info">{{list.info}}</div>
        <div class="name">- {{list.company}} -</div>
        <div class="time">
          <span>{{list.start}}</span>
          <span>{{list.end}}</span>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ['data']
}
</script>

<style lang="scss" scoped>
  .box{
    overflow: hidden;
    padding: 1rem 0 4rem 6rem;

    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      position: relative;
      transition: all 0.5s linear;
      top:0;

      &:last-of-type{top:8rem}
      
      &:before{
        content: "";
        display: block;
        width: 0;
        height: 100%;
        border: 0.1rem dashed #333;
        position: absolute;
        top: 0;
        left:3rem;
      }

      li{
        margin: 0 6rem 6rem;
        position: relative;
        padding: 1rem 2rem;
        background-color: #BDBDBD;
        color:#000;
        border-radius: 1rem;
        line-height: 2rem;
        width: 80%;
      }

      li > span{
        content: "";
        display: block;
        width: 0;
        height: 100%;
        border:0.1rem solid #333;
        position: absolute;
        top:0;
        left:-3rem;

        &:before,&:after{
          content: "";
          display: block;
          width: 1rem;
          height: 1rem;
          border-radius: 50%;
          background:#e97e22;
          border:0.2rem solid #333;
          position: absolute;
          left:-0.75rem;
        }

        &:before{top:-1rem}
        &:after{top:95%}
      }
    }

    .title{
      text-transform: uppercase;
      font-weight: 700;
      margin-bottom: 0.5rem
    }

    .text-info:first-letter{text-transform: capitalize;line-height: 1.7}

    .name{
      margin-top: 1rem;
      text-transform: capitalize;
      font-style: italic;
      text-align: right;
      margin-right: 2rem
    }

    .time span{
      position: absolute;
      left: -100px;
      color:#333;
      font-size:80%;
      font-weight: bold;

      &:first-child{top:-1.6rem}
      &:last-child{top:94%}
    }
  }

  @media only screen and (min-width: 992px) {
    .box {
      margin: auto;
      width: 50%;
    }
  }
</style>

