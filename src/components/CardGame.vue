<template>
  <div>
    <h1>{{ title }}</h1>
    <button type="button" @click="shuffle">Shuffle</button>
    <Player :name="player1" :cards="player1cards" />
    <Player :name="player2" :cards="player2cards" />
    <Player :name="player3" :cards="player3cards" />
    <Player :name="player4" :cards="player4cards" />
  </div>
</template>

<script>
import Player from "./Player.vue";

export default {
  name: 'CardGame',
  components: {
    Player,
  },
  data() {
    return {
      title: "start game",
      player1: "Alice",
      player1cards: ["♣10", "♣8", "♠3", "♦A", "♣9", "♣3", "♠A"],
      player2: "Bob",
      player2cards: ["♥4", "♦5", "♣5", "♦2", "♦8", "♦K", "♦9"],
      player3: "Carol",
      player3cards: ["♦Q", "♥7", "♠9", "♠J", "♠7", "♠Q", "♠6"],
      player4: "Eve",
      player4cards: ["♥A", "♠10", "♥5", "♦10", "♣6", "♣4", "♠2"],
    };
  },
  methods: {

    shuffle() {
      console.log("SHUFFLE");
    },
    deal() {
      console.log("SHUFFLE");
    },
    turn() {
      console.log("SHUFFLE");
    },
  },
};
</script>

<style scoped>

</style>

