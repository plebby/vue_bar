<template>
  <v-container>
    <v-row v-for="(drink, i) in menu.drinks" :key="i">
      <p>{{drink.name}}</p>
      <img
        :src="drink.image"
      />
    </v-row>
  </v-container>
</template>

<script>
import drinkList from '@/assets/drinks.json'

export default {
  name: 'PageHome',
  data () {
    return {
      menu: drinkList
    }
  }
}
</script>>
