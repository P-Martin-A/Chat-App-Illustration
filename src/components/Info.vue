<template>
  <div class="info">
    <h1 class="title">Simple booking</h1>
    <p class="text"> Stay in touch with our dog walkers through the chat interface. This makes it easy to discuss arrangements and make bookings. Once the walk has been completed you can rate your walker and book again all through the chat.</p>
  </div>
</template>

<script>
  export default {
    name: 'Info'
  }
</script>

<style scoped>
  .info{
    grid-area: Bottom;
    text-align: center;
  }

  .info .title{
    font-size: 3.5rem;
    margin-bottom: 1.5rem;
    color: var(--very-dark-desaturated-violet);
  }

  .info .text{
    font-size: 1.5rem;
    line-height: 2;
    color: var(--desaturated-dark-violet);
  }

  @media screen and (min-width: 900px){
    .info{
      height: 100%;
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: left;
    }

    .info .title, .info .text{
      width: 55%;
    }

    .info .text{
      line-height: 1.8;
      font-size: 1.2rem;
    }
  }
</style>