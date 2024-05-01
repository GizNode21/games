<template>
<div id="app">
    <div id="game">
        <Ga_me />
    </div>
    <div id="border" />
    <div id="input" >
        <Ch_at />
    </div>
</div>
</template>

<script>
    import Ch_at from './components/Ch_at.vue';
    import Ga_me from './components/Ga_me.vue';

    export default {
      name: 'App',
      components: {
        Ch_at,
        Ga_me
      }
    }
</script>

<style>
  #app {
    font-family: "Trebuchet MS", Helvetica, Arial, "sans-serif";
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: left;
    background-color: black;
    color: cyan;
    display: flex;
  }
  #game {
    width: 50vw;
    height: 100vh;
  }
  #border {
    border-right: 2px solid cyan;
  }
  #input {
    width: 50vw;
    height: 50vh;
  }
  @media (max-width: 1000px) {
    #app {
      flex-direction: column;
    }
    #game {
      width: 100vw;
      height: 50vh;
    }
    #input {
      width: 100vw;
      height: 50vh;
    }
  }
</style>
