<template>
  <button @click="decrementProps()">-</button>
</template>

<script>
export default {
  props: {
    handleDecrementCount: {
      type: Function,
      required: true,
    },
  },
  methods: {
    decrementProps() {
      this.handleDecrementCount()
    },
  },
}
</script>
