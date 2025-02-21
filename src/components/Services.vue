<script setup>
  import { ref } from 'vue'
import Transport from '../assets/transportes-1.webp'
import { Transition } from 'vue';

  const algo = ref(true)
</script>

<template>
  <section>
    <header>
      <h1>Nuestro servicios</h1>
    </header>

    <button @click="algo = !algo">Button</button>
    <Transition>
    <article v-show="algo">
        <h3>Transporte de mercancias</h3>
        <div class="info-container">
          <picture>
            <img :src=Transport alt="image">
          </picture>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officiis dolor illum commodi ex architecto error iure, quas iste molestiae nulla?</p>
        </div>
    </article>
  </Transition>
    <article>
      <h3>Servicios de logistica</h3>
      <div class="info-container">
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officiis dolor illum commodi ex architecto error iure, quas iste molestiae nulla?</p>
          <picture>
            <img :src=Transport alt="image">
          </picture>
        </div>
    </article>

    <article>
      <h3>Servicios de logistica</h3>
      <div class="info-container">
          <picture>
            <img :src=Transport alt="image">
          </picture>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officiis dolor illum commodi ex architecto error iure, quas iste molestiae nulla?</p>
        </div>
    </article>

  </section>
</template>

<style scoped>
  section {
    margin-inline: 20px;
  }

  h1 {
    text-align: center;
    margin-block: 50px;
  }

  article {
    margin-bottom: 30px;
  }

  h3 {
    margin-bottom: 40px;
  }

  .info-container {
    display: flex;
    justify-content: space-between;

    & p {
      align-content: center;
      width: 50%;
      padding: 35px;
    }
  }

  img {
    max-width: 100%;
    max-height: 50%;
    width: 730px;
    max-height: 400px;
    border-radius: 15px;
  }

  .v-enter-active,
  .v-leave-active {
    transition: opacity 0.5s ease-in-out;
  }
  
  .v-enter-from,
  .v-leave-to {
    opacity: 0;
  }
</style>