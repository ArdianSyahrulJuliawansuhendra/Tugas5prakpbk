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
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qukz-lhxmo4v97cyc61",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Alogo"
          },
          {
            img: "https://down-id.img.susercontent.com/file/sg-11134201-22120-egegyfktoplve2",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Guitarist"
          },
          {
            img: "https://down-id.img.susercontent.com/file/sg-11134201-22120-7dbeevhhoplv97",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Borealis"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qul0-lhxmo4v9ilm237",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Ne Bona"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qul0-lhxmo4v9fsd00a",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Demeter"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qula-li0d97cke4icac",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Manbe"
          },
          {
            img: "https://down-id.img.susercontent.com/file/sg-11134201-22120-d65vxq3eoplvb4",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "BlueRage"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qula-li0d0hr3hxisb9",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Blait"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qul7-li0d0hr3m584e1",
            title: "Reus Shirt",
            harga: "Rp 200.000",
            description: "Bluece"
          },
          // Four new cards
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7qul8-li0d97ckqrmc67",
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
  