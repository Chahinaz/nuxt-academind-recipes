<template>
  <section class="recipes">
    <Recipe
      thumbnail="https://cac.img.pmdstatic.net/fit/http.3A.2F.2Fwww.2Ecuisineactuelle.2Efr.2Fvar.2Fcui.2Fstorage.2Fimages.2Frecettes-de-cuisine.2Fplat.2Fhamburgers.2Fburger-maison-283827.2F3698362-1-fre-FR.2Fburger-maison.2Ejpg/1200x600/crop-from/center/burger-maison.jpg"
      title="Homemade burger."
      id="1"
      previewText="Delicious homemade burger."></Recipe>

    <Recipe
      thumbnail="http://akispetretzikis.com/system/uploads/medium/data/8404/akis-petretzikis-burger.jpg"
      title="Homemade burgers."
      id="2"
      previewText="Super fat homemade burgers."></Recipe>
  </section>
</template>


<script>
  import Recipe from '@/components/Recipe.vue'

  export default {
    components: {
      Recipe
    }
  }
</script>



