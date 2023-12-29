<script setup>

  import DefaultLayout from './layouts/Default.vue'
  import Iris from './components/Iris.vue'
  import Tracklist from './components/Tracklist.vue'

  const tracks = [
    {
      name: "BL!NK",
      artist: "Frost Children",
      imgurl: "./elixir_rejection.jpg",
      colors: [
        '63905E',
        'D6BBAE',
        '86A35F',
        '4E654D',
        '101315'
      ]
    },
    {
      name: "A.D.H.D - Alice Gas Remix",
      artist: "Cowgirl Clue",
      imgurl: "./adhd.jpg",
      colors: [
        'F4F5F5',
        '959595',
        '000000',
        '060606',
        '131313'
      ]
    },
    {
      name: "My Agenda",
      artist: "Dorian Electra",
      imgurl: "./my_agenda.jpg",
      colors: [
        '495A54',
        'C9E0A7',
        '80A98F',
        '141C18',
        '061107'
      ]
    },
    {
      name: "F The World ",
      artist: "Dorian Electra",
      imgurl: "./my_agenda.jpg",
      colors: [
        '495A54',
        'C9E0A7',
        '80A98F',
        '141C18',
        '061107'
      ]
    },
    {
      name: "scawy monstews and nice spwites :3",
      artist: "Fraxiom",
      imgurl: "./scawy.jpg",
      colors: [
        '8B241C',
        '4A3527',
        '1D0302',
        'D77A7E',
        'B2B08F'
      ]
    },
    {
      name: "PHILIPP PLEIN",
      artist: "Haiyti",
      imgurl: "./philipp_plein.jpg",
      colors: [
        'AEB5C0',
        'B9ABBB',
        'FB4711',
        '708BA4',
        'E38275'
      ]
    },
    {
      name: "Edgelord",
      artist: "Dorian Electra",
      imgurl: "./my_agenda.jpg",
      colors: [
        '495A54',
        'C9E0A7',
        '80A98F',
        '141C18',
        '061107'
      ]
    },
    {
      name: "GET WHAT WE WANT",
      artist: "Frost Children",
      imgurl: "./getwhatwewant.jpg",
      colors: [
        '948783',
        '832A48',
        'BDD9FB',
        '63453C',
        '7579B1'
      ]
    },
    {
      name: "Black Rum",
      artist: "Cake Pop",
      imgurl: "black_rum.jpg",
      colors: [
        'E2289E',
        '6857B5',
        'FFFFFF',
        '000000',
        '6D283C'
      ]
    },
    {
      name: "ILoveUIHateU",
      artist: "Playboi Carti",
      imgurl: "wlr.png",
      colors: [
        '000000',
        'FEFEFE',
        'D2C7C7',
        '1E1919',
        'CE0A0A'
      ]
    }
  ]

</script>

<template>

  <DefaultLayout>
    <div class="main-panel" id="left-panel">
      <Iris/>
      <div id="description">This is your Iris. An iridescent morphing collection of all the colors that make up the album artwork for your favorite music. Change the timeframe you want to pull from on the right.</div>
    </div>
    <div class="main-panel" id="right-panel">
      <ul id="timeframes">
        <li class="timeframe" id="monthly"><a>1 Month</a></li>
        <li class="timeframe"><a>6 Months</a></li>
        <li class="timeframe"><a>All Time</a></li>
      </ul>
      <Tracklist id="tracklist" :tracks="tracks"/>
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
    color: var(--primary-accent);
    /* box-shadow: 0px 2px var(--text-accent); */
  }

  #tracklist {
    height: 400px;
    width: 450px;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 40px;
    margin: 0 auto 0 auto;
  }


</style>
