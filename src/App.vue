<template>
  <div>
    <button @click="increment()">＋</button>
    <button @click="reset()">{{counter}}</button>
    <button @click="decrement()">ー</button>
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
    },
    decrement () {
      if (this.counter > 0) {
        this.counter -= 1
      }
    }
  }
}
</script>