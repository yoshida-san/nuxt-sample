<template>
  <label v-text="count"></label>
</template>

<script>
export default {
  props: {
    count: {
      type: Number,
      default: 0,
    },
  },
}
</script>
