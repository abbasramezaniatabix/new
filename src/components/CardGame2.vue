<template>
  <section class="cardgame">
  <card
  v-for="(card, index) in cardList"
  :key="card-$(index)"
  :value="card"
  />
  </section>
</template>
<script>
export default {
  name: 'App',
  components:{
    card
  },
  setup(){
    const cardList = []

    for(let i = 0; i < 52; i++) {
      cardList.push(i)
    }
  return { cardList
  }

  }
  
}
</script>

