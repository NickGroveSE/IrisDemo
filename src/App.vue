<script setup>

import DefaultLayout from './layouts/Default.vue'
import Iris from './components/Iris.vue'

</script>

<template>

  <DefaultLayout>
    <div class="main-panel" id="left-panel">
      <Iris/>
      <div id="description">This is your Iris. An iridescent morphing collection of all the colors that make up the album artwork for your favorite music. Change the timeframe you want to pull from on the right.</div>
    </div>
    <div class="main-panel" id="right-panel">
      <ul id="timeframes">
        <li class="timeframe" id="monthly"><a>Last 30 Days</a></li>
        <li class="timeframe"><a>Last 3 Months</a></li>
        <li class="timeframe"><a>Last Year</a></li>
      </ul>
    </div>
  </DefaultLayout>

</template>

<style scoped>

  /* Panel Styling */
  .main-panel {
    height: 100%;
    position: relative;
    display: inline-block;
    vertical-align: top;
  }

  #left-panel {
    width: calc(50% - 100px);
    margin-left: 100px;
  }

  #right-panel {
    width: calc(50% - 100px);
    margin-right: 100px;
  }

  /* Intra-Panel Styling*/
  #description {
    width: 300px;
    height: 80px;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 50px;
    margin: 0 auto 0 auto;
    padding: 5px;
    font-size: 14px;
    text-align: center;
  }

  #timeframes {
    height: 30px;
    width: 390px;
    margin: 20px auto 0 auto;
    padding: 0%;
    list-style: none;

  }

  .timeframe {
    width: 130px;
    line-height: 30px;
    display: inline-block;
    font-size: 18px;
    text-align: center;
  }

  a {
    text-decoration: none;
  }

  #monthly {
    border-bottom: 2px solid var(--primary-accent);
    /* box-shadow: 0px 2px var(--text-accent); */
  }


</style>
