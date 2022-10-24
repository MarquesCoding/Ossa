<script>
  import svelteLogo from './assets/svelte.svg'
  import OSSALogo from './assets/logo.svg'
  import { fade } from 'svelte/transition'
  import Counter from './lib/Counter.svelte'
  import { transition_in } from 'svelte/internal';
  import { slide } from 'svelte/transition';

  let y;   
  let showFade = false 

  $: console.log(y)


  function toggleFade() {
    showFade = !showFade
  }

  window.addEventListener('scroll', () => {
    const scrollableDiv = document.getElementById("scroll")
    console.log(scrollableDiv)
  })
</script>




<svelte:window bind:scrollY={y}/>




<main>

  <div class="header">
    <img src="src\assets\static\pattern-background.jpg" alt="" class="background_image">
    <img src="src\assets\static\logo-fff.png" alt="">
  </div>

  
  <div class="section__buttons">
    <div class="section__button">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M8.25 6.75L12 3m0 0l3.75 3.75M12 3v18"
        />
      </svg>
    </div>
    <div class="section__button">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M15.75 17.25L12 21m0 0l-3.75-3.75M12 21V3"
        />
      </svg>
    </div>
  </div>


  <div class="main__content">


    <section class="hidden" style="padding: 200px;"> 
      <div class="textLeft">
        <div class="text hidden">
          <h2>
            Almost every
          </h2>
        </div>
        <div class="text hidden">
          <h2>
            business in the
          </h2>
        </div>
        <div class="text hidden">
          <h2>
            country is a
          </h2>
        </div>
        <div class="text hidden">
          <h2>
            small business
          </h2>
        </div>
      </div>
    </section>


    <section class="hidden">
      <div class="textRight">
        <div class="text hidden" transition:fade>
          <h2>Small businesses</h2>
        </div>
        <div class="text hidden">
          <h2>provide services</h2>
        </div>
        <div class="text hidden">
          <h2>that make our day</h2>
        </div>
        <div class="text hidden">
            <h2>to day lives work.</h2>
        <div class="text hidden" >
          <h2 style="font-weight: bolder;">They are the</h2>
        </div>
        <div class="text hidden">
          <h2 style="font-weight: bolder;">lifeblood of our</h2>
        </div>
        <div class="text hidden">
          <h2 style="font-weight: bolder;">economy.</h2>
        </div>
      </div>
    </section>

    <section class=hidden>
      <div class="textRight" >
          <div class="text hidden">
            <h2>But advertising agencies</h2>
          </div>
          <div class="text hidden" >
            <h2>don't even give them the</h2>
          </div>
          <div class="text hidden">
            <h2>time of day.</h2>
          </div>
        </div>
      <div class="textRight">
          <div class="text hidden" >
            <h2 style="font-weight: bolder;">They only want to help</h2>
          </div>
          <div class="text hidden" >
            <h2 style="font-weight: bolder;">the big businesses.</h2>
          </div>
      </div>
  </section>
    
  <section class="hidden">
    <div class="textRight">
      <div class="text hidden">
          <h2>So those millions</h2>
      </div>
      <div class="text hidden">
          <h2>of small business</h2>
      </div>
      <div class="text hidden">
          <h2>owners have to</h2>
      </div>
      <div class="text hidden">
          <h2>tackle the</h2>
      </div>
      <div class="text hidden">
          <h2>confusing world of digital advertising,</h2>
      </div>
      <div class="text hidden">
          <h2 style="font-weight: bolder;">alone.</h2>
      </div>
    </div>
    <div class="textLeft">
      <div class="text hidden">
          <h2> 
            But now, they
          </h2>
      </div>
      <div class="text hidden">
        <h2 style="font-weight: bold"> 
          have OSSA
        </h2>
    </div>
    </div>
  </section>

  <section class="hidden"> 
    <div class="textLeft">
      <div class="text hidden">
        <h2> 
          OSSA has a clever
        </h2>
      </div>
    <div class="text hidden">
      <h2> 
        advertising brain
      </h2>
    </div>
      <div class="pulse">
        <img src="src\assets\static\brain-01.png" alt="" style="position: relative; left: 33%;" >
      </div>
    </div>
  </section>


  <section class="hidden">
    <div class="textLeft">
      <div class="text hidden">
        <h2> 
          It knows the science
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          behind how ads work
        </h2>
      </div>
    </div>
  </section>

  <section>
    <div class="textLeft">
      <div class="text hidden">
        <h2> 
          And uses artificial
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          intelligence to 
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          automatically 
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          create the right 
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          advertising for
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          any small 
        </h2>
      </div>
      <div class="text hidden">
        <h2> 
          business
        </h2>
      </div>
    </div>
  </section>

  <section>
    <div class="sectionCenter">
      <div class="text hidden">
        <h2>
          Its quite magical!
        </h2>
      </div>
    </div>
  </section>
    
  
  <section class="hidden">
    <div class="sectionCenter">
      <div class="text hidden">
        <h2>
          So small businesses can
        </h2>
      </div>
      <div class="text hidden">
        <h2>
          attract more customers and
        </h2>
      </div>
      <div class="text hidden">
        <h2>
          become bigger businesses. 
        </h2>
      </div>
      <div class="text hidden">
        <h2>
          Growth for them and growth
        </h2>
      </div>
      <div class="text hidden">
        <h2>
          for the economy. 
        </h2>
      </div>
    </div>
  </section>


  <section class="hidden">
    <img src="src\assets\logo.svg" alt="" class="large__logo blur">
    <img src="src\assets\logo.svg" alt="" class="large__logo">
    <div class="sectionCenter" style="margin-top: -400px;">
      <div class="text hidden">
        <h2>
          Welcome to OSSA.
        </h2>
      </div> 
      <div class="text hidden">
        <h2> Online Self-Service Advertising</h2>
      </div>
    </div>
  </section>


  <div class="footer">
    <div class="top__bar"></div>
    <img src="src\assets\logo.svg" alt="" style="position: relative; left:20%; top: 150px;" class="footerlogo">
    <div style="position:relative; margin-left: 1500px; margin-bottom: 20px;" class="footertext">
      <nav>
        <h3>
          Apply
        </h3>
        <h3>
          Contact us
        </h3>
        <h3>
          Investment Opportunities
        </h3>
      </nav>
    </div>
    <div style="position: relative; margin-left: 41%;">
      <h3>
        @ Copyright 2022. All rights reserved.
      </h3>
    </div>
      </div>

  </div>
  
  
</main>

<style>

</style>
