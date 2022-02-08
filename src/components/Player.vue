<template>
  <div class="container">
    <h3>{{ name }}{{ cards }}</h3>
    <div class="btn"><button type="button" @click="shuffle">Shuffle</button>
  
  </div>
  </div>
</template>

<script>

export default {
  name: 'Player',
  props: {
    name: String,
    cards: Array,
    deck: Array
  },
  methods: {
    shuffle() {
      console.log("SHUFFLE");
    },
  },

};
</script>

<style scoped>

.btn{
  display: block;
  margin: 0 auto;
  text-align: left;
  padding-top: 30px;
  margin-bottom: 0 !important;
}
</style>

