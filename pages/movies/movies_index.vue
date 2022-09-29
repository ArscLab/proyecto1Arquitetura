<!-- pages/books_index.vue -->
<template>
    <div class="container">
     <h3 style="margin-top: 15px">Peliculas</h3>
     <p>Lista</p>
     <ul>
       <ContentList path="/movies" v-slot="{ list }">
          <li v-for="movie in list" :key="movie._path">
           <NuxtLink :to="movie._path"> <img :src="movie.img" width="100"> {{ movie.name }}</NuxtLink>
          </li>
        </ContentList>
     </ul>
   </div>
  </template>