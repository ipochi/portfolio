<template>
  <div id="app">
    <frontpage></frontpage>
  </div>
</template>


<script>

import FrontPageComponent from './components/FrontPageComponent.vue';

export default {

  name: 'app',

  components : {
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
