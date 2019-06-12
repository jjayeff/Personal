<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col span-1-of-2">
          <ul class="footer-nav">
            <li><a href="#">About us</a></li>
            <li><a href="#">Blog</a></li>
            <li><a href="#">Press</a></li>
            <li><a href="#">iOS App</a></li>
            <li><a href="#">Android App</a></li>
          </ul>
        </div>
        <div class="col span-1-of-2">
          <ul class="social-links">
            <li><a href="#"><i class="icon ion-logo-facebook"></i></a></li>
            <li><a href="#"><i class="icon ion-logo-twitter"></i></a></li>
            <li><a href="#"><i class="icon ion-logo-googleplus"></i></a></li>
            <li><a href="#"><i class="icon ion-logo-instagram"></i></a></li>
          </ul>
        </div>
      </div>
      <div class="row">
        <p>
            Copyright &copy; 2015 by Omnifood. All rights reserved.
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  footer {
    background-color: #333;
    color: #fff;

    p {
      color: #888;
      text-align: center;
      padding-bottom: 10px;
    }
  }

  .footer-nav {
    list-style: none;
    float: left;

    li {
      display: inline-block;
      padding: 20px;

      a {
        &:link,
        &:visited {
          color: #888;
          text-decoration: none;
          transition: color 0.2s;
        }

        &:hover,
        &:active {
          color: #ddd;
        }
      }
    }
  }

  .social-links {
    list-style: none;
    float: right;

    li {
      display: inline-block;
      padding: 20px;

      a {
        &:link,
        &:visited {
          color: #888;
          font-size: 150%;
          transition: color 0.2s;
        }

        &:hover,
        &:active {
          color: #ddd;
        }
      }
    }
  }
</style>
