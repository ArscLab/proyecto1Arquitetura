// components/global/Author.vue
<template>
  <div>
    <div>
      <h4>Author</h4>
      <p>{{ author.name }}</p>
      <p>{{ author.bio }}</p>
    </div>
  </div>
</template>
<script>
  export default {
    props: {
      author: {
        type: Object,
        required: true
      }
    }
  }
</script>