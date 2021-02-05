<template>
  <div>
    <div>
      <CounterLabel :count="count" />
    </div>
    <div>
      <IncrementButton :handle-increment-count="incrementCount" />
      <DecrementButton :handle-decrement-count="decrementCount" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    count: {
      type: Number,
      default: 0,
    },
    incrementCount: {
      type: Function,
      required: true,
    },
    decrementCount: {
      type: Function,
      required: true,
    },
  },
}
</script>
