<script setup>
/* Избранное */
import { ref, onMounted } from 'vue'
import axios from 'axios'

import CardList from '../components/CardList.vue'

const favorites = ref([])

onMounted(async () => {
  try {
    const { data } = await axios.get(
      'https://4e37a2182929b119.mokky.dev/favorites?_relations=items'
    )
    console.log(data)
    favorites.value = data.map((obj) => obj.item)
  } catch (err) {
    console.log(err)
  }
})
</script>

<template>
  <h2 class="text-3xl font-bold mb-8">Избранное</h2>

  <CardList :items="favorites" is-favorites />
</template>
