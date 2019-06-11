<template>
    <section class="abount-me">
      <div class="container">
        <div class="row">
          <div class="col span-1-of-3 image-box">
            <img class="image" src="https://www.cm108.com/bbb/uploads/monthly_2016_04/571f6f5abe5bb_cccc_1-(1).jpg.97e02b4b4d5cc2c538c9811bff9c7777.jpg" alt="">
            <h3>ekkawit lertkrai<br>developer & programmer</h3>
            <p>+66 8998 49157</p>
            <p>ekkawit.lertkrai@gmail.com</p>
            <p>bangkok thailand.</p>
          </div>
          <div class="col span-2-of-3">
            <h2>who am i</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus repellat quia obcaecati quam quaerat. Id, magni doloremque, excepturi minus debitis eaque quia odit beatae soluta minima corrupti alias quo totam?</p>
            <div class="education">
              <h2>My Education</h2>
              <div class="row education-content">
                <img class="col span-1-of-2" src="https://upload.wikimedia.org/wikipedia/th/6/62/KMUTNB-LOGO.jpg" alt="">
                <div class="col span-1-of-2">
                  <h3>Computer Science, Bachelor's Degree</h3>
                  <h5>KMUTNB, BANGKOK, THAILAND, 2014-2019</h5>
                </div>
              </div>
            </div>
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
  .abount-me {
    margin: 50px;
  }
  .image-box {
  text-align: center;

    .image {
      height: auto;
      width: 50%;
      border-radius: 50%;
    }

    h3 {
      text-transform: uppercase;
      margin-top: 10px;
      margin-bottom: 20px;
    }
  }
    
  h2 {
    font-size: 180%;
    word-spacing: 2px;
    text-align: center;
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

  .education {
    margin-top: 50px;
  }
  .education-content {
    img {
      height: 100px; 
      width: auto;
      vertical-align: middle; /* | top | bottom */
      padding: 0px 40px; 
    }

    div {
      margin: 15px;
      padding: 10px;
      padding-left: 30px;
      border-left: 2px solid #e97e22;

      h3 {
        font-size: 120%;
        padding: 0px 5px;
      }

      h5 {
        padding: 5px 5px;
      }
    }
    
    }
</style>
