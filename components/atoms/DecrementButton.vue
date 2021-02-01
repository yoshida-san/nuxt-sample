<template>
  <button @click="decrement"><slot /></button>
</template>

<script>
export default {
  methods: {
    decrement() {
      this.$store.commit('sampleDir/moreDir/sample/decrement')
    },
  },
}
</script>
