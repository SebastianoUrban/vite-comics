<template>
  <div class="wrapper flex">
    <div class="links flex">
      <div >
        <h3>DC Comics</h3>
        <ul>
          <li v-for="item in footerList['dcComics']">
            {{ item }}
          </li>
        </ul>
        <h3>SHOP</h3>
        <ul>
          <li v-for="item in footerList['shop']">
            {{ item }}
          </li>
        </ul>
      </div>

      <div>
        <h3>DC</h3>
        <ul>
          <li v-for="item in footerList['dc']">
            {{ item }}
          </li>
        </ul>
      </div>

      <div>
        <h3>SITES</h3>
        <ul>
          <li v-for="item in footerList['sites']">
            {{ item }}
          </li>
        </ul>
      </div>
    </div>

    <img src="../assets/img/dc-logo-bg.png" alt="">
  </div>
</template>

<script>
import { useAttrs } from 'vue';

  export default {
    data() {
      return {
        footerList: {
          dcComics : ['Characters', 'Comics', 'Movies', 'Tv', 'Games', 'Videos', 'News'],
          shop : ['Shop DC', 'Shop DC Collectibles'],
          dc : ['Terms Of Use', 'Privacy Policy (New)', 'Ad Choies', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshop', 'CPSC Cetificates', 'Ratings', 'Shop Help', 'Contact Us'],
          sites : ['DC', 'DC Kids', 'DC Universe', 'DC Power Visa']
        }
      }
    },
  }
</script>

<style scoped>
  div.wrapper{
    height: 450px;
    justify-content: space-between;
    overflow-y: hidden;

  }

  img {
    height: 500px;
    transform: translateY(-25px);
  }

  h3 {
    color: white;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    margin-top: 0.5rem;
    color: rgb(151, 151, 151);
  }

  div.links div {
    padding-right: 3rem;
  }
</style>