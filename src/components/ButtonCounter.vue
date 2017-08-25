<template>
  <button v-on:click="increment">
    {{ counter }}
  </button>
</template>

<script>
export default {
  name: 'buttonCounter',
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increment: function() {
      this.counter++
      this.$emit('increment')
    }
  },
}

</script>

<style>

</style>
