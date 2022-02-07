<template>
  <div>
    <h3>{{ name }}{{ cards }}</h3>
    <button type="button" @click="shuffle">Shuffle</button>
  </div>
</template>

<script>

export default {
  name: 'Player',
  props: {
    name: String,
    cards: Array,
  },
  methods: {
    shuffle() {
      console.log("SHUFFLE");
    },
  },

};
</script>

<style scoped>

</style>

