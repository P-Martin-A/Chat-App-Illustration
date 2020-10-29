<template>
  <Container />
</template>

<script>
  import Container from './layouts/Container'

  export default {
    name: 'App',
    components: {
      Container
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;700&display=swap');

  *, *::before, *::after{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  :root{
    --very-dark-desaturated-violet: rgb(62, 39, 83);
    --desaturated-dark-violet: rgb(110, 93, 126);
    --dark-grayish-violet: rgb(163, 157, 170);
    --light-violet: rgb(136, 56, 255);
    --moderate-violet: rgb(146, 65, 200);
    --light-magenta: rgb(233, 66, 255);
    --very-light-magenta: rgb(229, 112, 255);
    --pale-violet: rgb(216, 158, 255);
    --grayish-blue: rgb(198, 202, 205);
    --light-grayish-violet: rgb(245, 243, 247);
    --white: rgb(255, 255, 255);
  }

  html{
    font-size: 10px;
  }

  html body{
    font-family: 'Rubik', sans-serif;
    background-color: var(--light-grayish-violet);
  }

  html body h1, html body h4, html body b{
    font-weight: 700;
  }

  html body p{
    font-weight: 500;
  }

  html body span{
    font-weight: 400;
  }
</style>