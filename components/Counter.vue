<template>
  <div>
    <div>
      <CounterLabel />
    </div>
    <div>
      <IncrementButton text="+" @welcome="say" />
      <DecrementButton><slot>Decrement</slot></DecrementButton>
      <SayButton @sayCount="say" />
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    say(val) {
      alert(val)
    },
  },
}
</script>
