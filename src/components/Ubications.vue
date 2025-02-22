<script setup>

</script>

<template>
  <section id="ubication" v-motion-slide-visible-bottom>
    <header>
      <h1>Ubicacion</h1>
    </header>

      <article>
        <iframe
        src='https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1410.6084304503352!2d-78.48157423108933!3d-0.15801586139696877!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x91d59b1c21b265cf%3A0x903c3fc62c679a27!2sTorres%20del%20Inca%20-%20Departamento!5e0!3m2!1ses!2sec!4v1724785322907!5m2!1ses!2sec'
        width='900'
        height='500'
        loading='lazy'
      />
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

  article {
    margin-top: 30px;
    display: flex;
    justify-content: center;
  }
  
  iframe {
    margin-bottom: 50px;
  }
</style>