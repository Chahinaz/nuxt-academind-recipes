<template>
  <section class="recipes">
    <Recipe
      v-for="recipe in recipes"
      :key="recipe.id"
      :thumbnail="recipe.thumbnail"
      :title="recipe.title"
      :id="recipe.id"
      :previewText="recipe.previewText"></Recipe>
  </section>
</template>


<script>
  import Recipe from '@/components/Recipe.vue'

  export default {
    components: {
      Recipe
    },
  }
</script>



