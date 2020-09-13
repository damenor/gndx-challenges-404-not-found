<template>
  <div class="not-found__container">

    <div class="not-found__container-image">
      <img v-bind:src="image" alt="scarecrow"/>
    </div>
    
    <div class="not-found__container-text">
      <h3>I have bad news for you</h3>
      <p>
        The page you are looking for might be removed or is temporarily unavailable
      </p>
      <button>back to homepage</button>
    </div>

  </div>
</template>

<script>

  import image from '../../assets/images/Scarecrow.png'

  export default {
    name: 'NotFoundContainer',
    data() {
      return { image }
    }
  }

</script>

<style scoped>

  @import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');
  
  .not-found__container {
    display: flex;
    align-items: center;
  }

  .not-found__container-text,
  .not-found__container-image {
    display: flex;
    flex: 1;
    height: 100%;
    padding: 4rem;
    animation: var(--animation-fade-in);
  }

  .not-found__container-image {
    align-items: center;
  }
  
  .not-found__container-image img {
    width: 100%;
  }

  .not-found__container-text {
    flex-direction: column;
    justify-content: center;
  }

  .not-found__container-text h3 {
    margin: 0;
    color: var(--color-danger);
    font-size: 6rem;
    font-family: 'Creepster', cursive;
  }

  .not-found__container-text p {
    max-width: 24rem;
    margin: 3rem 0;
    color: var(--color-grey);
    font-size: 2rem;
    line-height: 2.5rem;
  }

  .not-found__container-text button {
    max-width: 15rem;
    padding: 2rem;
    color: var(--color-light);
    text-transform: uppercase;
    background-color: var(--color-dark);
    border: none;
    cursor: pointer;
    transition: all .2s;
  }

  .not-found__container-text button:active {
    padding: 1.5rem;
    margin-top: 0.5rem;
    margin-bottom: 0.5rem;
    transform: scale(0.95);
  }

  @media (max-width: 1200px) {
    .not-found__container-text,
    .not-found__container-image {
      padding: 2rem;
    }
    .not-found__container-text h3 {
      font-size: 4rem;
    }
    .not-found__container-text p {
      font-size: 1.5rem;
      line-height: 2rem;
    }
  }

  @media (max-width: 940px) {
    .not-found__container {
      flex-direction: column;
    }
    .not-found__container-text {
      align-items: center;
    }
    .not-found__container-text h3 {
      font-size: 2.5rem;
      text-align: center;
    }
    .not-found__container-text p {
      font-size: 1.25rem;
      text-align: justify;
    }
  }

</style>