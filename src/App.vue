<script setup>
import DcHeader from './components/DcHeader.vue'
import DcMain from './components/DcMain.vue'
import DcFooter from './components/DcFooter.vue'
</script>

<template>
  <header>
    <DcHeader/>
  </header>

  <main>
    <DcMain/>
  </main>

  <footer>
    <DcFooter/>
  </footer>
</template>

<style scoped>
  main {
    background-color: #1c1c1c;
    width: 100%;
  }
  footer {
    background-image: url(./assets/img/footer-bg.jpg);
  }
</style>
