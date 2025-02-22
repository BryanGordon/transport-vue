<script setup>
  import Transport from '../assets/transportes-1.webp'
  import Facebook from '../icons/Facebook.vue';
  import Instagram from '../icons/Instagram.vue';
  import Whatsapp from '../icons/Whatsapp.vue';
</script>

<template>
  <section id="contactos" v-motion-slide-visible-bottom>
    <header>
      <h1>Contactos</h1>
    </header>

    <article>
      <h3>Sede principal</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti quidem aliquam labore debitis sit quis nesciunt voluptatum temporibus alias molestiae odio, suscipit delectus commodi numquam laborum eaque rem ea quam.</p>
      
      <div class="container-img">
        <img :src=Transport alt="image">
      </div>
    </article>

    <article>
      <h3>Nuestras redes sociales</h3>
      <div class="container-icons">
        <a href="https://facebook.com">
          <Facebook />
        </a>
        <a href="https://instagram.com">
          <Instagram />
        </a>
        <a href="https://whatsapp.com">
          <Whatsapp />
        </a>
      </div>
    </article>
  </section>
</template>

<style scoped>
  section {
    margin-inline: 30px;
  }

  h1 {
    text-align: center;
    margin-block: 50px;
  }

  h3 {
    margin-bottom: 40px;
  }

  article {
    margin-bottom: 30px;
  }

  .container-img {
    width: 50%;
    padding: 60px;
    margin: 0 auto;
  }

  img {
    max-width: 100%;
    border-radius: 12px;
  }

  .container-icons {
    display: flex;
    justify-content: space-evenly;
  }

</style>