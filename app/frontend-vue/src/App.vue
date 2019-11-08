<template>
  <div id="app">
    <img id="amber-logo" alt="Amber logo" src="./assets/amber-logo.png"> <br>
    <img id="vue-logo" alt="Vue logo" src="./assets/vue-logo.png">
    <HelloWorld msg="Welcome to Amber with Vue"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
  #app {
    font-family: Dosis, Open Sans, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  #amber-logo {
    height: 200px;
    width: 200px;
    padding-right: 115px;
  }
  #vue-logo {
    height: 175px;
    width: 175px;
    margin-top: -125px;
    padding-left: 115px;
  }
  .amber-text {
    font-family: Dosis, Open Sans, sans-serif;
    color: #e68a00;
  }
  .vue-text {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    color: #42b983;
  }

  @font-face {
    font-family: 'Dosis';
    font-style: normal;
    font-weight: 300;
    src: url(https://fonts.gstatic.com/s/dosis/v16/HhyaU5sn9vOmLzloC_WoEoZK.woff2) format('woff2');
    unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
  }
  @font-face {
    font-family: 'Dosis';
    font-style: normal;
    font-weight: 600;
    src: url(https://fonts.gstatic.com/s/dosis/v16/HhyaU5sn9vOmLzloC_WoEoZK.woff2) format('woff2');
    unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
  }
</style>
