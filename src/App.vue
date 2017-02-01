<template>
  <div>
    <button @click="increment()">{{counter}}</button>
    <button @click="reset()">reset</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      counter: 0
    }
  },
  methods: {
    increment () {
      this.counter += 1
    },
    reset () {
      this.counter = 0
    }
  }
}
</script>