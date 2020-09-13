<template>
  <div class="not-found__header">
    <h2>404 not found</h2>
  </div>
</template>

<script>
export default {
  name: 'NotFoundHeader'
}
</script>

<style scoped>
  .not-found__header {
    padding: 0 2rem;
    animation: var(--animation-fade-in);
  }
  @media (max-width: 940px) {
    .not-found__header {
      text-align: center;
    }
  }
</style>