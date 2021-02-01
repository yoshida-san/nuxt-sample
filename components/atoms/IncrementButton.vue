<template>
  <button @click="increment">{{ text }}</button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: 'Increment',
    },
  },
  methods: {
    increment() {
      this.$store.commit('sampleDir/moreDir/sample/increment')
    },
  },
}
</script>
