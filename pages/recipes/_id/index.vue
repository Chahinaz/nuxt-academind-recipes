<template>
  <section class="single-recipe">
    <h1>{{ recipe.title }}</h1>
    <div>
      <img class="recipe-image" :src="recipe.thumbnail" :alt="recipe.title">
    </div>
    <p>{{ recipe.descriptionText }}</p>
  </section>
</template>

<script>
  export default {
    asyncData(context) {
      return new Promise((resolve, reject) => {
        setTimeout(() => {
          resolve({
            recipe: [
              {
                id: "1",
                title: "Homemade burger.",
                previewText: "Delicious and fast-made homemade burger.",
                descriptionText: "Description...",
                thumbnail: "https://cac.img.pmdstatic.net/fit/http.3A.2F.2Fwww.2Ecuisineactuelle.2Efr.2Fvar.2Fcui.2Fstorage.2Fimages.2Frecettes-de-cuisine.2Fplat.2Fhamburgers.2Fburger-maison-283827.2F3698362-1-fre-FR.2Fburger-maison.2Ejpg/1200x600/crop-from/center/burger-maison.jpg"
              },
              {
                id: "2",
                title: "Homemade burgers.",
                previewText: "Super fat and tasty homemade burgers.",
                descriptionText: "Description...",
                thumbnail: "http://akispetretzikis.com/system/uploads/medium/data/8404/akis-petretzikis-burger.jpg"
              }
            ].find(el => el.id === context.params.id)
          })
        }, 1500)
      })
    }
  }
</script>

<style>
  .single-recipe {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 2rem;
    flex-flow: column wrap;
  }

  .recipe-image {
    width: 100%
  }
</style>
