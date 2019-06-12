<template>
  <section class="contact">
    <div class="container">
      <h3>contact</h3>
      <div class="row">
        <form method="post" action="#" class="contact-form">
          <div class="row">
            <div class="col-md-4">
              <label for="name">Name</label>
            </div>
            <div class="col-md-8">
              <input type="text" name="name" id="name" placeholder="Your name" required>
            </div>
          </div>
          <div class="row">
            <div class="col-md-4">
              <label for="email">Email</label>
            </div>
            <div class="col-md-8">
              <input type="email" name="email" id="email" placeholder="Your email" required>
            </div>
          </div>
          <div class="row">
            <div class="col-md-4">
              <label for="email">Subject</label>
            </div>
            <div class="col-md-8">
              <input type="email" name="subject" id="subject" placeholder="Your subject" required>
            </div>
          </div>
          <div class="row">
            <div class="col-md-4">
              <label>Drop us a line</label>
            </div>
            <div class="col-md-8">
              <textarea name="message" placeholder="Your message"></textarea>
            </div>
          </div>
          <div class="row">
            <div class="col-md-4">
              <label>&nbsp;</label>
            </div>
            <div class="col-md-8">
              <app-button name='Send it!!'/>
            </div>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
  import appButton from '../core/Button1.vue';
  export default {
    components: {
      appButton
    }
  }
</script>

<style lang="scss">
  .contact {
    padding: 5rem;
    h3 {
      word-spacing: 0.2rem;
      margin-bottom: 3rem;
      letter-spacing: 0.1rem;
      text-align: center;
      font-weight: 300;
      text-transform: uppercase;
      &:after {
        display: block;
        height: 0.1rem;
        background-color: #e97e22;
        content: "";
        width: 10rem;
        margin: 0 auto;
        margin-top: 2rem;
      }
    }

    .contact-form {
      width: 60%;
      margin: 0 auto;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 7px;
      border-radius: 3px;
      border: 1px solid #ccc;
    }

    textarea {
      height: 100px;
    }
  }
</style>

