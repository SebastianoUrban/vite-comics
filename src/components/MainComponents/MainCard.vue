<template>
  <div class="card">
    <img :src="thumb" alt="pic">
    <h4>{{ series }}</h4>
  </div>
</template>

<script>
import { stringifyExpression } from '@vue/compiler-core';

  export default {
    props : {
      thumb : String,
      price : String,
      series : String,
      type : String
    }
  }
</script>

<style scoped>
  img {
    object-fit: cover;
    width: 100%;
    height: 200px;
  }

  div.card {
    width: calc(100% / 6);
    overflow: hidden;
    padding: 15px;
    box-sizing: border-box;
  }

  h4 {
    color: white;
  }
</style>