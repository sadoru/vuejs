<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button v-on:click="toggle">toggle</button>
    <h2 v-show="showText">{{ text }}</h2>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      // msg: 'Welcome to Your Vue.js App'
      msg: 'hello test',
      text: 'test text',
      showText: false
    }
  },
  methods: {
    toggle: function () {
      this.showText = !this.showText;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
/* ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
} */
</style>
