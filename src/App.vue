<template>
  <main>
    <header>
      <h2>Star Wars Characters</h2>
    </header>
    <div>
      <ul>
        <li v-for="{name,  species, img} in characters" :key="name">
          <h3>{{ name }}</h3>
          <p>{{ species }}</p>
          <img :src="img.src" :alt="img.alt">
        </li>
      </ul>
    </div>
  </main>
</template>

<script setup>
const characters = [
  {
    name: "Goongyoo",
    side: "Light",
    species: "actor",
    img: {
      src: "https://img.marieclairekorea.com/2021/10/mck_615ea554d4d12.jpg",
      alt: "actor",
    },
  },
  {
    name: "Exo",
    side: "Dark",
    species: "singer",
    img: {
      src: "https://cdn.i-scmp.com/sites/default/files/d8/images/methode/2021/05/11/1fd3dd62-b205-11eb-93b7-03206dd91175_image_hires_173202.jpg",
      alt: "singer",
    },
  },
  {
    name: "dockbockie",
    side: "light",
    species: "want some food?",
    img: {
      src: "https://wooltariusa.com/cdn/shop/products/1000000016_detail_189.jpg?v=1690483823",
      alt: "Grogu looking for snacks",
    },
  },
];
</script>

<style scoped>
img {
  width: 200px;
}
</style>