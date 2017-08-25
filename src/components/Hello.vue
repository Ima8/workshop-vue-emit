<template>
  <div id="counter-event-example">
    <p>{{ total }}</p>
    <buttonCounter @increment="incrementTotal"></buttonCounter>
    <buttonCounter @increment="incrementTotal"></buttonCounter>
  </div>
</template>

<script>
import buttonCounter from '@/components/ButtonCounter'


export default {
  name: 'hello',
  components: {
    buttonCounter
  },
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      total: 0
    }
  },
  methods: {
    incrementTotal: function() {
      this.total++
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
