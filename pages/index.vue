<template>
  <div class="container">
    <section>
      <Counter />
    </section>
  </div>
</template>

<script>
export default {
  // layout: 'sampleLayout',
  middleware: 'sampleMiddleware',
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
