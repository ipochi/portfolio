<template lang="html">

  <div>
    <section class="section has-text-centered is-paddingless has-padding">
        <figure class="image is-128x128 image-cs">
          <img class="is-img-circle" src="https://media.licdn.com/mpr/mpr/shrinknp_400_400/AAEAAQAAAAAAAAx9AAAAJDc0MGE3Njk2LTFhYjEtNDZmMy04MzQ3LTViNGQwZGUxYjk5OA.jpg">
        </figure>

      <h2 class="title">
        <strong>IMRAN POCHI</strong>
      </h2>
      <h6 class="subtitle flair-font">
        Developer . Versatile . Learner
      </h6>
    </section>

    <section class="section has-text-centered">
      <div class="container has-text-centered">
        <h6 class="subtitle flair-font">
          Get in touch to get the ball rolling.
        </h6>
      </div>
    </section>

    <section class="section is-paddingless">
      <nav class="level is-mobile">

        <div class="level-item has-text-centered">

        </div>

        <div class="level-item has-text-centered">
          <div>
            <a href="mailto:pochiimran@yahoo.co.in">
              <span>
                <i class="fa fa-envelope-o fa-3x has-text-dark"></i>
              </span>
            </a>
          </div>
        </div>

        <div class="level-item has-text-centered">
          <div>
            <a v-on:click="showMobileNumber">
              <span>
                <i class="fa fa-mobile fa-3x"></i>
              </span>
            </a>
          </div>
        </div>

        <div class="level-item has-text-centered">
          <div>
            <a href="https://github.com/ipochi" target="_blank">
                <i class="fa fa-github fa-3x has-text-dark"></i>
            </a>
          </div>
        </div>

        <div class="level-item has-text-centered">
          <div>
            <a href="https://www.linkedin.com/in/imranpochi" target="_blank">
                <i class="fa fa-linkedin-square fa-3x has-text-dark"></i>
            </a>
          </div>
        </div>
        <div class="level-item has-text-centered">
          <div>
            <a href="https://www.facebook.com/imran.pochi" target="_blank">
              <i class="fa fa-facebook fa-3x has-text-info"></i>
            </a>
          </div>
        </div>

        <div class="level-item has-text-centered">

        </div>
      </nav>

      <transition enter-active-class="animated slideInUp" leave-active-class ="animated slideOutDown">
      <div class=" container has-text-centered is-primary is-bold" v-show="isShowMobileNumber">
        <strong>+91 782 925 6229</strong>
        <button class="delete" v-on:click="closeNotification"></button>
      </div>
    </transition>

    </section>

  </div>
</template>

<script>
export default {
  data() {
    return {
      isShowMobileNumber : false
    }
  },

  methods : {
    showMobileNumber() {
      this.isShowMobileNumber = ! this.isShowMobileNumber;
    },
    closeNotification() {
      this.isShowMobileNumber = false;
    }
  },
}
</script>

<style lang="css">

.image-cs {
  margin-right: auto;
  margin-left: auto;
}

.is-img-circle {
  border-radius: 50%;
}

.has-padding {
    margin-top: 20px;
}

</style>
