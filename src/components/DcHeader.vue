<template>
  <div class="wrapper">
    <img src="../assets/img/dc-logo.png" alt="Logo Dc">
    <ul>
      <li v-for="navItem in navList">
        {{ navItem.toUpperCase()}}
      </li>
    </ul>
  </div>
  
</template>

<script>
  export default {
    data() {
      return {
        navList: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
      }
    },
  }
</script>

<style  scoped>
  div.wrapper{
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
    padding: 15px 0;
  }

  ul {
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  li {
    margin-left: 15px;
    font-weight: bold;
    font-size: 0.9rem;
  }
</style>