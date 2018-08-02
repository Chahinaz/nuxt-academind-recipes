<template>
  <section class="recipes">
    <article class="recipe">
      <div class="thumbnail" style="background-image: url(https://cac.img.pmdstatic.net/fit/http.3A.2F.2Fwww.2Ecuisineactuelle.2Efr.2Fvar.2Fcui.2Fstorage.2Fimages.2Frecettes-de-cuisine.2Fplat.2Fhamburgers.2Fburger-maison-283827.2F3698362-1-fre-FR.2Fburger-maison.2Ejpg/1200x600/crop-from/center/burger-maison.jpg)"></div>
        <h1>Title 1</h1>
        <p>Some usefull text</p>
    </article>

    <article class="recipe">
      <div class="thumbnail" style="background-image: url(https://www.atelierdeschefs.com/media/recette-e17282-burger-au-cheddar-potatoes-au-melange-cajun.jpg)"></div>
        <h1>Title 2</h1>
        <p>Still, that's usefull text</p>
    </article>
  </section>
</template>


<script>

</script>


<style scoped>
  .recipes {
    display: flex;
    flex-flow: row wrap; /*responsive style*/
    justify-content: center; /*flew box property*/
    align-items: center; /*flew box property*/
  }

  .recipe{
    box-sizing: border-box;
    width: 280px;
    padding: 8px;
    border: 1px solid #fff;
    box-shadow: 0 2px 2px #aaa;
    margin: 10px;
  }

  .thumbnail {
    background-position: center;
    background-size: cover;
    width: 100%;
    height: 200px;
  }
</style>
