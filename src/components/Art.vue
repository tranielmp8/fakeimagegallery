<template>
  <div>
    <div class="container">
      <div v-for="image in images" :key="image.id" >
        {{ image.title }}
        {{ image.printPrice }}
        <img :src="image.img" alt="Tie Art">
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'
  export default {
    setup(){
      const images = ref([
        {
          "id": 1,
          "title": "Demon Slayer",
          "description": "just something to talk about. cool stuff",
          "printPrice": "$500.00",
          "uniquePrice": "$1250.00",
          "img": '/images/demon_slayer.jpg'
        },
        {
          "id": 2,
          "title": "Demon Slayer",
          "description": "just something to talk about. cool stuff",
          "printPrice": "$500.00",
          "uniquePrice": "$1250.00",
          "img": '/images/luffy.jpg'
        },
        {
          "id": 3,
          "title": "Demon Slayer",
          "description": "just something to talk about. cool stuff",
          "printPrice": "$500.00",
          "uniquePrice": "$1250.00",
          "img": '/images/bleach.jpg'
        },
        {
          "id": 4,
          "title": "Naruto",
          "description": "just something to talk about. cool stuff",
          "printPrice": "$500.00",
          "uniquePrice": "$1250.00",
          "img": '/images/naruto.jpg'
        },
      ])

      return {images}
    }
  }
</script>