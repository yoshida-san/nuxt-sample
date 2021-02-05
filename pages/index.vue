<template>
  <div class="container">
    <section>
      <Counter
        :count="$store.state.sampleDir.moreDir.sample.counter"
        :increment-count="incrementCount"
        :decrement-count="decrementCount"
      />
    </section>
  </div>
</template>

<script>
export default {
  // layout: 'sampleLayout',
  middleware: 'sampleMiddleware',
  methods: {
    incrementCount() {
      this.$store.commit('sampleDir/moreDir/sample/increment')
    },
    decrementCount() {
      this.$store.commit('sampleDir/moreDir/sample/decrement')
    },
  },
}
</script>

<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
