<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="public/WhatsApp Image 2024-05-26 at 01.33.33_a29939c4.jpg" class="carousel-img" />
      <q-carousel-slide :name="2" img-src="public/WhatsApp Image 2024-05-26 at 01.33.33_8c723a61.jpg" class="carousel-img" />
      <q-carousel-slide :name="3" img-src="public/WhatsApp Image 2024-05-26 at 01.33.33_ca00a96d.jpg" class="carousel-img" />
      <q-carousel-slide :name="4" img-src="public/WhatsApp Image 2024-05-26 at 01.33.33_b33c936a.jpg" class="carousel-img" />
    </q-carousel>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1)
    }
  }
}
</script>

<style scoped>
.carousel-img {
  width: 100%; /* Menggunakan lebar 100% agar gambar terlihat responsif */
  height: 1080px; /* Menggunakan ketinggian otomatis agar gambar tetap proporsional */
  max-height: 100px; /* Atur ketinggian maksimum agar gambar tidak terlalu besar */
  background-size: contain; /* Menggunakan contain untuk memastikan gambar tetap proporsional */
  background-position: center; /* Posisikan gambar di tengah-tengah */
}
</style>
