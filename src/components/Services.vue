<script setup>
  import Transport from '../assets/transportes-1.webp'
</script>

<template>
  <section>
    <header>
      <h1>Nuestro servicios</h1>
    </header>

    <article>
        <h3>Transporte de mercancias</h3>
        <div class="info-container">
          <picture>
            <img :src=Transport alt="image">
          </picture>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officiis dolor illum commodi ex architecto error iure, quas iste molestiae nulla?</p>
        </div>
    </article>

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

    & p{
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
</style>