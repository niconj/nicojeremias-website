<template>
  <div id="app">
    <PresentationCard msg="Welcome to Your Vue.js App"/>
    <footer>
      <SocialContact></SocialContact>
    </footer>
  </div>
</template>

<script>
import PresentationCard from './components/Presentation-Card.vue'
import SocialContact from './components/Social-Contact.vue'

export default {
  name: 'app',
  components: {
    PresentationCard,
    SocialContact
  }
}
</script>

<style lang="scss">
  @import '_variables.scss';

  body {
    margin: 0;
    background: $background-color;
  }

  #app {
    font-family: 'Quicksand', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: $primary-color;
  }
</style>
