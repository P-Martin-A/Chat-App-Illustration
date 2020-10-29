<template>
  <div class="container"> 
    <div class="gradient"></div>
    <Phone />
    <Info />
  </div>
</template>

<script>
  import Phone from '../components/Phone'
  import Info from '../components/Info'

  export default {
    name: 'Container',
    components: {
      Phone,
      Info
    }
  }
</script>

<style scoped>
  .container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding: 4rem;
  }

  .container .gradient{
    z-index: -1;
    position: absolute;
    top: 0;
    left: -30%;
    width: 30rem;
    height: 50rem;
    clip-path: circle(72% at 33% 38%);
    background: linear-gradient(to top, var(--light-violet), var(--moderate-violet));
  }

  @media screen and (min-width: 900px){
    .container{
      flex-direction: row;
      height: 100vh;
    }

    .container .gradient{
      top: 0;
      left: 0;
    }
  }
</style>