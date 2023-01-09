<template>
  <div class="wrapper flex-centered">
    <img src="../assets/img/dc-logo.png" alt="Logo Dc">
    <ul class="flex-centered">
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
    justify-content: space-between;
    height: 120px;
  }

  img {
    height: 80%;
  }

  ul {
    list-style-type: none;
    justify-content: space-between;
  }

  li {
    margin-left: 20px;
    font-weight: bold;
    font-size: 0.8rem;
  }
</style>