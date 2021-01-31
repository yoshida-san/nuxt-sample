<template>
  <button @click="sayCount">Say</button>
</template>

<script>
export default {
  methods: {
    sayCount() {
      this.$emit('sayCount', this.$store.state.counter)
    },
  },
}
</script>
