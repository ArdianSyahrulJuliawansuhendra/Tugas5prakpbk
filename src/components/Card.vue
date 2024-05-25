<template>
    <div class="q-pa-md">
      <div class="grid-wrapper q-gutter-md">
        <q-card v-for="(card, index) in cards" :key="index" class="my-card">
          <img :src="card.img" class="card-img">
          <q-card-section>
            <div class="text-h6">{{ card.title }}</div>
            <div class="text-subtitle2">{{ card.harga }}</div>
          </q-card-section>
          <q-card-section class="q-pt-none">
            {{ card.description }}
          </q-card-section>
        </q-card>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    setup() {
      return {
        cards: [
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7quky-li0d3vafsrn4f9",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Alogo"
          },
          {
            img: "src/assets/IMG-20240526-WA0035.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Guitarist"
          },
          {
            img: "src/assets/IMG-20240526-WA0036.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Borealis"
          },
          {
            img: "src/assets/IMG-20240526-WA0037.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Ne Bona"
          },
          {
            img: "src/assets/IMG-20240526-WA0038.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Demeter"
          },
          {
            img: "src/assets/IMG-20240526-WA0039.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Manbe"
          },
          {
            img: "src/assets/IMG-20240526-WA0040.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "BlueRage"
          },
          {
            img: "src/assets/IMG-20240526-WA0041.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Blait"
          },
          {
            img: "src/assets/IMG-20240526-WA0042.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Bluece"
          },
          // Four new cards
          {
            img: "public/WhatsApp Image 2024-05-26 at 01.33.33_8c723a61.jpg",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Russel"
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .grid-wrapper {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 16px;
  }
  
  .my-card {
    width: 100%;
    max-width: 100%;
    background-image: linear-gradient(163deg, #01204E 10%, #028391 100%);
    border-radius: 5px;
    transition: all .3s;
    cursor: pointer;
  }
  
  .card-img {
    width: 100%;
    height: auto;
  }
  
  .my-card:hover {
    transform: scale(0.98);
  }
  
  @media (max-width: 600px) {
    .grid-wrapper {
      grid-template-columns: 1fr;
    }
  
    .my-card {
      margin-bottom: 16px;
    }
  }
  </style>
  