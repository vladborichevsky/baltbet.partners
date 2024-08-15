
<template>
  <div class="intro">

    <div class="intro_media">
      <video loop class="intro__media-video" autoplay muted playsinline preload="yes" src="/video.mp4" type="video/mp4"/>
    </div>

    <a href="https://baltbetpartners.partner.alanbase.com/registration" class="logo">
      <img src="/logo.png" alt="Иконка">
    </a>

    <a href="https://baltbetpartners.partner.alanbase.com/registration" class="become_a_partner">
      Cтать партнёром
    </a>

  </div>
</template>



<script setup>

</script>



<style scoped>
  .intro {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 100vw;
  }

  .intro_media {
    position: absolute;
    top: 0;
    right: 0;
    height: 100%;
    width: 100%;
    overflow: hidden;
  }

  .intro__media-video {
    position: absolute;
    top: 50%;
    left: 50%;
    min-width: 100%;
    min-height: 100%;
    transform: translate(-50%, -50%);
    object-fit: cover
  }


  .become_a_partner {
    text-decoration: none;
    cursor: pointer;
    position: absolute;
    top: 80%;
    right: 50%;
    transform: translateX(50%) ;
    background-color: var(--green-color);
    color: var(--white-color);
    padding: 10px 15px;
    font-size: 20px;
    font-weight: 500;
    border: 2px solid var(--green-color);
    border-radius: 10px;
  }

  .become_a_partner:hover {
    transition: all .5s;
    border: 1px solid var(--black-color);
  }

  .logo {
    cursor: pointer;
    position: absolute;
    border: none;
    top: 5%;
    left: 5%;
  }

  .logo img {
    width: 200px;
  }

  @media(max-width: 992px) {
    .logo img {
      width: 150px;
    }

    .become_a_partner {
      font-size: 18px;
    }
  }

  @media(max-width: 767px) {
    .become_a_partner {
      font-size: 16px;
    }
  }
  
  @media(max-width: 576px) {
    .logo img {
      width: 150px;
    }

    .become_a_partner {
      padding: 7px 10px;
      font-size: 15px;
      font-weight: 500;
      width: 170px;
      text-align: center;
    }
  }

</style>
