<template>
  <button @click="incrementProps()">+</button>
</template>

<script>
export default {
  props: {
    handleIncrementCount: {
      type: Function,
      required: true,
    },
  },
  methods: {
    incrementProps() {
      this.handleIncrementCount()
    },
  },
}
</script>
