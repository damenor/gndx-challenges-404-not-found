<template>
  <NotFound/>
</template>

<script>
import NotFound from './components/NotFound/NotFound.vue'

export default {
  name: 'App',
  components: {
    NotFound
  }
}
</script>

<style>

  @import url('https://fonts.googleapis.com/css2?family=Kufam&display=swap');

  * {
    box-sizing: border-box;
  }

  *:focus {
    outline: none;
  }

  body, #app {
    min-height: 100vh;
    margin: 0;
    font-family: 'Kufam', cursive;
  }

</style>
