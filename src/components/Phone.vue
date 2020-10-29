<template>
  <div class="phone">
    <div class="sound"></div>
    <header class="header">
      <div class="profile">
        <img class="icon" src="../assets/images/bxs-chevron-left.svg" alt="<">  
        <img class="avatar" src="../assets/images/avatar.jpg" alt="Person">
        <div class="content">
          <h4 class="title">Samuel Green</h4>
          <span class="subtitle">Available to Walk</span>
        </div>
      </div>
      <img class="icon" src="../assets/images/bx-dots-vertical-rounded.svg" alt="...">
    </header>
    <main class="main">
      <span class="left">That sounds great. I’d be happy with that.</span>
      <span class="left">Could you send over some pictures of your dog, please?</span>
      <div class="dogs">
        <img src="../assets/images/dog-image-1.jpg" alt="Dog" class="dog">
        <img src="../assets/images/dog-image-2.jpg" alt="Dog" class="dog">
        <img src="../assets/images/dog-image-3.jpg" alt="Dog" class="dog">
      </div>
      <span class="right">Here are a few pictures. She’s a happy girl!</span>
      <span class="right">Can you make it?</span>
      <span class="left">She looks so happy! The time we discussed works. How long shall I take her out for?</span>
      <div class="price">
        <span class="circle"></span>
        <span class="text">30 minute walk</span>
        <b>$29</b>
      </div>
      <div class="price">
        <span class="circle"></span>
        <span class="text">1 hour walk</span>
        <b>$49</b>
      </div>
      <div class="message">
        <input type="text" placeholder="Type a message…"> 
        <img class="icon" src="../assets/images/bxs-chevron-right.svg" alt=">">
      </div>
    </main>
  </div>
</template>

<script>
  export default {
    name: 'Phone'
  }
</script>

<style scoped>
  .phone{
    position: relative;
    grid-area: Top;
    height: 50rem;
    width: 25rem;
    background-color: var(--light-grayish-violet);
    border: 1rem solid var(--white);
    border-radius: 2.5rem;
    box-shadow: 0 1rem 2.5rem var(--dark-grayish-violet);
    margin-bottom: 5rem;
  }

  .phone .sound{
    position: absolute;
    left: 50%;
    right: 50%;
    transform: translateX(-50%);
    background-color: var(--white);
    border-bottom-right-radius: 1.5rem;
    border-bottom-left-radius: 1.5rem;
    height: 2rem;
    width: 12rem;
  }

  .phone .header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 6.5rem;
    width: 100%;
    padding: 2rem .8rem 0 .8rem;
    border-top-right-radius: 1.5rem;
    border-top-left-radius: 1.5rem;
    border-bottom-right-radius: 1rem;
    border-bottom-left-radius: 1rem;
    background: linear-gradient(to right, var(--moderate-violet), var(--light-magenta));
  }

  .phone .header .profile{
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .phone .header .profile .avatar{
    width: 2.5rem;
    border-radius: 50%;
    border: 1px solid var(--white);
    margin-right: .5rem;
  }

  .phone .header .content .title{
    color: var(--white);
  }

  .phone .header .content .subtitle{
    color: var(--light-grayish-violet);
    opacity: .5;
  }

  .phone .main{
    padding: .8rem 1rem;
    display: flex;
    flex-direction: column;
  }

  .phone .main .left, .phone .main .right, .phone .main .price{
    padding: .5rem;
    margin-bottom: 1rem;
    width: 15rem;
    border-radius: .8rem;
  }

  .phone .main .left{
    align-self: flex-start;
    background-color: var(--grayish-blue);
    color: var(--light-magenta);
    opacity: .4;
  }

  .phone .main .dogs, .phone .main .right{
    align-self: flex-end;
  }

  .phone .main .dogs{
    margin-bottom: 1rem;
  }

  .phone .main .dogs .dog{
    margin: 0 .2rem;
    width: 4.5rem;
    border-radius: .8rem;
  }

  .phone .main .right{
    background-color: var(--white);
    color: var(--dark-grayish-violet);
  }

  .phone .main .price{
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: linear-gradient(to left, var(--moderate-violet), var(--light-magenta));
    color: var(--light-grayish-violet);
    padding: 1rem;
  }

  .phone .main .price .circle{
    border: 1px solid var(--light-grayish-violet);
    border-radius: 50%;
    height: 1.2rem;
    width: 1.2rem;
  }
  
  .phone .main .price b{
    color: var(--white);
  }

  .phone .main .message{
    position: relative;
    display: flex;
  }

  .phone .main .message input[type="text"]{
    font-size: 1.2rem;
    padding: 1rem;
    border: none;
    border-radius: 1rem;
    width: 100%;
  }

  .phone .main .message .icon{
    cursor: pointer;
    position: absolute;
    right: 1rem;
    top: .5rem;
    background-color: var(--very-dark-desaturated-violet);
    border-radius: 50%;
  }

  @media screen and (min-width: 900px){
    .phone{
      margin-right: 2rem;
    }
  }
</style>