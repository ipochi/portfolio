<template lang="html">
  <div>
    <section class="hero hero-image" v-bind:class="{'is-fullheight': isActive}">
      <div class="hero-head" v-if=" ! isActive">

        <nav class="nav">

          <div class="nav-left">
            <a class="nav-item" v-on:click="backToFullScreen">
              <span class="icon">
                <i class="fa fa-angle-double-down has-text-dark"></i>
              </span>
            </a>
          </div>
          <div class="nav-center">
            <a class="nav-item" v-on:click="swapComponent('aboutme')">
              <span class="subtitle">
                <i class="has-text-light">About</i>

              </span>
            </a>
            <a class="nav-item" v-on:click="swapComponent('aboutwork')">
              <span class="subtitle">
                <i class="has-text-light">Work</i>
              </span>
            </a>
            <a class="nav-item" v-on:click="swapComponent('contactme')">
              <span class="subtitle">
                <i class="has-text-light">Contact</i>
              </span>
            </a>
          </div>

          <div class="nav-right">
            <a class="nav-item" v-on:click="backToFullScreen">
              <span class="icon">
                <i class="fa fa-angle-double-down has-text-dark"></i>
              </span>
            </a>
          </div>
        </nav>

      </div>

  <!-- Hero content: will be in the middle -->
        <section class="hero-body" v-if="isActive">
          <div class="container has-text-centered">
            <div class="content is-large has-text-centered" v-show="isActive">
              <h2 class="title">
                <strong style="color:white">IMRAN POCHI</strong>
              </h2>
              <h6 class="subtitle flair-font" style="color:white">
                Developer . Versatile . Learner
              </h6>
            </div>
          </div>
        </section>
        <section class="hero-body" v-if="isActive">
          <div class="container">
            <div class="columns">
              <div class="column is-one-quarter">

              </div>
              <div class="column has-text-centered">
                <p class="heading has-text-light">About</p>
                <a v-on:click="swapComponent('aboutme')">
                    <i class="fa fa-user-circle-o fa-5x has-text-light"></i>
                </a>
              </div>
              <div class="column has-text-centered">
                <p class="heading has-text-light">Work</p>
                <a v-on:click="swapComponent('aboutwork')">
                  <i class="fa fa-briefcase fa-5x has-text-light"></i>
                </a>
              </div>
              <div class="column has-text-centered">
                <p class="heading has-text-light">Contact</p>
                <a v-on:click="swapComponent('contactme')">
                  <span>
                    <i class="fa fa-commenting-o fa-5x has-text-light"></i>
                  </span>
                </a>
              </div>
              <div class="column has-text-centered">
                <p class="heading has-text-light">Contact</p>
                <a v-on:click="swapComponent('contactme')">
                  <span>
                    <i class="fa fa-commenting-o fa-5x has-text-light"></i>
                  </span>
                </a>
              </div>
              <div class="column is-one-quarter">

              </div>
            </div>
          </div>
        </section>
    </section>

    <transition appear enter-active-class="animated bounceInUp">
      <div :is="currentComponent"></div>
    </transition>

   <!-- <maincontent v-if=" ! isActive"></maincontent> -->
</div>
</template>

<script>

import MainContent from './MainContent.vue';

import AboutMe from './AboutMeComponent.vue';
import AboutWork from './AboutWorkComponent.vue';
import ContactMe from './ContactMeComponent.vue';


export default {
  components : {
    maincontent : MainContent,
    aboutme : AboutMe,
    aboutwork : AboutWork,
    contactme : ContactMe
  },

  data() {
    return {
      isActive : true,
      currentComponent: null,
      componentsArray: ['aboutme', 'aboutwork' , 'contactme']
    }
  },
  methods : {
    backToFullScreen() {
      if( ! this.isActive) {
        this.isActive = true;
        this.currentComponent = null;
      }
    },
    changeActive() {
      this.isActive = ! this.isActive;
    },
    swapComponent(component){
      this.isActive = false;
      this.currentComponent = component;
    }
  }
}
</script>

<style lang="css">

/* Enter and leave animations can use different */
/* durations and timing functions.              */
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active for <2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}

.hero-image {
  background :  linear-gradient(

      rgba(252, 53, 76, 0.80),
      rgba(10, 191, 188, 0.80)
    /*
    rgba(26, 41, 128, 0.85),
    rgba(38, 208, 206, 0.85)
    */
    ), url('/src/assets/backgroundImage.jpg');

    /* Center and scale the image nicely */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  opacity: 0.8;

}

.flair-font {
  font-family: Georgia,"Lucida Sans",serif,;
  font-style: italic;
}

.title-font {
  font-family: "Helvetica Neue",Helvetica,sans-serif;
}
</style>
