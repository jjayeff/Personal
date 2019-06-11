<template>
  <section class="experience">
    <div class="container">
      <h2>Experience</h2>
      <div class="row">
        <h1>2017</h1>
        <div>
          <h1>Intership</h1>
          <h3>ITTP, BANGKOK, THAILAND </h3>
          <ul>
            <li>React/Redux</li>
            <li>React Native</li>
            <li>NoSQL</li>
          </ul>
        </div>
      </div>
      <div class="row">
          <h1>2018</h1>
          <div>
            <h1>Programmer</h1>
            <h3>TopTrader, BANGKOK, THAILAND </h3>
            <ul>
              <li>C++</li>
              <li>C#/ASP.net</li>
              <li>MySQL</li>
            </ul>
          </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .experience {
    background-color: #f4f4f4;
    padding: 50px;
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
  }

</style>
