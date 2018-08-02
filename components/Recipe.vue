<template>
  <section class="recipes">
    <article class="recipe">
      <div class="thumbnail" :style="{backgroundImage: 'url(' + thumbnail + ')'}"></div>
      <h1>Title</h1>
      <p>Some usefull text</p>
    </article>
  </section>
</template>

<script>
  export default {
    props: ["thumbnail", "title", "previewText"]
  }
</script>

<style scope>
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
