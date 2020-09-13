<template>
  <div class="not-found">
    <NotFoundHeader />
    <NotFoundContainer />
    <NotFoundFooter />
  </div>
</template>

<script>

  import NotFoundContainer from './NotFoundContainer'
  import NotFoundFooter from './NotFoundFooter'
  import NotFoundHeader from './NotFoundHeader'

  export default {
    name: 'NotFound',
    components: {
      NotFoundContainer,
      NotFoundFooter,
      NotFoundHeader
    }
  }

</script>

<style scoped>

  .not-found {
    height: 100vh;
    display: grid;
    grid-template-rows: 3rem auto 3rem;
  }

</style>
