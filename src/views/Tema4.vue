<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 4
      h1 Programación de comportamientos relativos a la mecánica de videojuego
    .row.justify-content-center
      .col-lg-10
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema4/1.png')})`}"
          )
          .bloque-texto-g__texto.p-5
            p.mb-0 La interacción del jugador con los objetos del videojuego desempeña un papel muy importante en las mecánicas del videojuego, ya que así puede saber el estado actual del nivel, los elementos que ha recolectado para su inventario, qué nivel de vida le queda, entre otros muchos aspectos más.
    .row.mt-5
      .col-5
        .row.align-items-center
          .col-2
            img(src='@/assets/curso/tema1/ico.svg', alt='Texto que describa la imagen')
          .col-10
            h4.mb-0 Interactividad UI Recolección de ítems de juego
    p.mt-4 Una de las principales actividades que se deben cumplir en la gran mayoría de mecánicas es la recolección de objetos en el escenario; esto hace que el jugador pueda recoger pociones mágicas, pociones de salud e incluso municiones para sus armas.
    p Continuando con las colisiones del Character Controller, en el siguiente video se explica la creación de un sistema de recolección y conteo que se visualiza en la interfaz de usuario (UI).
    .video
      iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    
</template>

<script>
export default {
  name: 'Tema4',
  components: {},
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
