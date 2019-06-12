<template>
    <section class="abount-me">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <div class="image-box">
              <img class="image" src="https://www.cm108.com/bbb/uploads/monthly_2016_04/571f6f5abe5bb_cccc_1-(1).jpg.97e02b4b4d5cc2c538c9811bff9c7777.jpg" alt="">
              <h6>ekkawit lertkrai<br>developer & programmer</h6>
              <p>+66 8998 49157</p>
              <p>ekkawit.lertkrai@gmail.com</p>
              <p>bangkok thailand.</p>
            </div>
          </div>
          <div class="col-md-8">
            <h3>who am i</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus repellat quia obcaecati quam quaerat. Id, magni doloremque, excepturi minus debitis eaque quia odit beatae soluta minima corrupti alias quo totam?</p>
            <div class="education">
              <h3>My Education</h3>
              <div class="row education-content">
                <img class="col-xs-3" src="https://upload.wikimedia.org/wikipedia/th/6/62/KMUTNB-LOGO.jpg" alt="">
                <div class="col-xs-9">
                  <h4>Computer Science, Bachelor's Degree</h4>
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
    margin: 5rem;
  }
  .image-box {
    text-align: center;
    padding: 0.5rem;

    .image {
      height: auto;
      width: 50%;
      border-radius: 50%;
    }

    h6 {
      text-transform: uppercase;
      margin-top: 1rem;
      margin-bottom: 2rem;
    }

    p {
      padding: 0.2rem 0;
    }
  }
    
  h3 {
    word-spacing: 0.2rem;
    text-align: center;
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

  .education {
    margin-top: 5rem;
  }
  .education-content {
    img {
      height: 8rem; 
      width: auto;
      vertical-align: middle; /* | top | bottom */
    }

    div {
      padding: 1.5rem;

      h4 {
        font-size: 120%;
        padding: 0 0.5rem;
      }

      h5 {
        font-size: 100%;
        padding: 0.5rem 0.5rem;
        font-weight: 300;
      }
    }
  }

  @media only screen and (max-width: 768px) {
    .image-box {
      margin-left: 190px
    }
  }

  @media only screen and (max-width: 700px) {
    .image-box {
      margin-left: 155px
    }
  }

  @media only screen and (max-width: 650px) {
    .image-box {
      margin-left: 125px
    }
  }

  @media only screen and (max-width: 600px) {
    .image-box {
      margin-left: 65px
    }
  }
</style>
