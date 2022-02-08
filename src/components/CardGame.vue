
<template>
  
  <div>
    <img src ="assets./file1.png">
    <div class="title"><h1>{{ title }}</h1></div>
    <button type="button" @click="shuffle">Shuffle</button>
    <div class="p1"><player :name="player1" :cards="player1cards" /></div>
    <div class="p2"><Player :name="player2" :cards="player2cards" /></div>
    <div class="p3"><Player :name="player3" :cards="player3cards" /></div>
    <div class="p4"><Player :name="player4" :cards="player4cards" /></div>
    <div class="p4"><Player :name="player5" :cards="player5cards" /></div>
 
      <button @click="shuffleDeck" class="button is-primary"> Shuffle <i class="fas fa-random"></i></button>

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
      player5: "asdad",
      player5cards: ["♥A", "♠10", "♥5", "♦10", "♣6", "♣4", "♠2"],

      
    };
  },
  

/*  ranks: ['A', '2', '3', '4', '5', '6', '7', '8', '9', '10', 'J', 'Q', 'K'],
    suits: ['♥','♦','♠','♣'],
    cards: [],
    suitColor: {
    '♠': 'black',
      '♣': 'black',
      '♦': 'red',
      '♥': 'red',
    },
*/
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
.title {
  border-radius: 10px;
  background-color: chocolate;
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  margin: 20px;
  padding-top: 30px;
  margin-bottom: 0 !important;
  
}
.p1 {
  font-family: 'helvetica neue', helvetica, sans-serif;
            letter-spacing: 1px;
            text-transform: uppercase;
            text-align: center;
            border: 2px solid rgba(0, 0, 200, 0.6);
            background: rgba(0, 0, 200, 0.3);
            color: rgba(0, 0, 200, 0.6);
            box-shadow: 1px 1px 2px rgba(0, 0, 200, 0.4);
            border-radius: 10px;
            padding: 3px 10px;
            display: inline-block;
            cursor: pointer;
}
.p2{
  background-color: cornflowerblue;
}
.p3{
  background-color: crimson;
}
.p4{
  background-color: darkgrey ;
}
</style>

