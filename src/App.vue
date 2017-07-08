<template>
  <div id="app">
    <frontpage></frontpage>
  </div>
</template>


<script>

import NavComponent from './components/AboutMeComponent.vue';
import MainContent from './components/MainContent.vue';
import FrontPageComponent from './components/FrontPageComponent.vue';

export default {

  name: 'app',

  components : {
    maincontent : MainContent,
    frontpage : FrontPageComponent
  },

  data() {
    return {
    }
  },
  methods : {
  },

}
</script>

<style lang="css">

</style>
