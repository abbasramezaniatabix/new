

<template>
  <div>
    <h1>{{ title }}</h1>
    <button type="button" @click="shuffle">Shuffle</button>

    <h3>{{ player1 }}{{ player1cards }}</h3>
    <hr />
    <h3>{{ player2 }}{{ player2cards }}</h3>
    <button type="button" @click="shuffle">Shuffle</button>
    <hr />
    <h3>{{ player3 }}{{ player3cards }}</h3>
    <button type="button" @click="shuffle">Shuffle</button>
    <hr />
    <h3>{{ player1 }} {{ player4cards }}</h3>
    <button type="button" @click="shuffle">Shuffle</button>
  </div>
</template>



<script>

export default {
  name: 'CardGame',
  data(){
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







<!--
<template>
  <div>
    
    <button id="drawbtn">DRAW A CARD</button>
  
  <div class="card template">
    <span class="rank">10</span>
    <span class="suit">Hearts</span>
</div>
    
  </div>
</template>
<script>
var suits = ["hearts", "diams", "clubs", "spades"];
var ranks = [2, 3, 4, 5, 6, 7, 8, 9, 10, "J", "Q", "K"];
var deck = [];
this.$emit("event-name");
init;

function init() {
  makeDeck();

  this.$emit(newFunction());
  "#drawbtn".click(function () {
    var myCard = drawcard();
    if (myCard) {
      makecard(myCard.suit, myCard.rank);
    } else {
      alert("no more cards in de deck");
    }
  });

  function newFunction() {
    return "event-name";
  }
}
function makeDeck() {
  deck = [];
  //for each type of suit
  for (var i = 0; i < suits.length; i++) {
    //and for each rank
    for (var j = 0; j < ranks.length; j++) {
      //make a card
      var card = {};
      card.suit = suits[i];
      card.rank = ranks[j];
      deck.push(card);
    }
  }
  console.log("Made a new deck of", deck.length, "cards");
  console.log(deck);
}
function drawcard() {
  var card;
  if (deck.length > 0) {
    var randIndex = Math.floor(Math.random() * deck.length);
    card = deck.splice(randIndex, 1)[0];
  }
  return card;
}
function makecard(suit, rank) {
  var card = this.$emit("event-name");
  ".card.template".clone();
  card.removeclass("template");

  card.find(".rank").html(rank);
  card.find(".suit").html("&" + suit + ";");

  if (suit === "hearts" || suit === "diams") {
    card.addclass("red");
  }
  this.$emit("event-name");
  "body".apend(card);
}

</script>

<style scoped>
.card {
  display: inline-block;
  text-align: center;
  margin: 5px;
  padding: 18px 15px 0 15px;
  width: 70px;
  height: 40px;

  font-size: 22px;
  background: color #999;
  border: solid 1px black;
}
.red {
  background-color: #e55451;
  border: solid 1px #8c001a;
  color: #8c001a;
}
.template {
  display: none;
}
</style>
-->
