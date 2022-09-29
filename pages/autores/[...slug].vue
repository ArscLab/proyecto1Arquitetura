<!-- pages/movies/[...slug].vue -->
<template>
    <div class="container">
     <div class="row">
       <ContentDoc v-slot="{doc}">
       <div class="three columns">
         <img width="200" :src="doc.img">
       </div>
       <div class="six columns">
         <h4>{{doc.name}}</h4>
        
          <pre></pre>
         <h5>Description</h5>
          <p>{{doc.description}}</p>
       </div>
       <NuxtLink :to="'/movies/movies_index'">Volver</NuxtLink>
       <div class="two columns"></div>
      </ContentDoc>
     </div>
   </div>
  </template>