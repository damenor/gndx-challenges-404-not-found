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

  :root {
    --color-dark: #333333;
    --color-danger: #ff6b6b;
    --color-grey: #666;
    --color-light: #f2f2f2;
    --animation-fade-in: fadeIn .6s forwards;
  }

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

  @keyframes fadeIn {
    0% { opacity: 0 }
    100% { opacity: 1 }
  }

</style>
