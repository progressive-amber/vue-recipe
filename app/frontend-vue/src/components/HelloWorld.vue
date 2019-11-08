<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>Feel free to refer to the docs!</h3>
    <p>
      <a class="vue-text" href="https://vuejs.org/v2/guide/" target="_blank" rel="noopener">Vue.js documentation</a> <br>
      <a class="amber-text" href="https://docs.amberframework.org/amber/" target="_blank" rel="noopener">Amber documentation</a>
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
    font-weight: lighter;
  }
</style>
