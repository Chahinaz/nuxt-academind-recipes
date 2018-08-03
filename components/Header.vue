<template>
  <header>
    <nav>
      <ul>
        <li><nuxt-link to="/">Staring Page</nuxt-link></li>
        <li><nuxt-link to="/recipes">Recipes</nuxt-link></li>
      </ul>
    </nav>
  </header>
</template>


<style>
  header {
    width: 100%;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  li {
    margin: 0 10px;
  }
</style>
