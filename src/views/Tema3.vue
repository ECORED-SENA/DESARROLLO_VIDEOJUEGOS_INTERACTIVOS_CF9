<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h1 Programación de eventos disparadores (interacción con el entorno)
    .row.justify-content-center
      .col-lg-10
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema3/1.png')})`}"
          )
          .bloque-texto-g__texto.p-5
            p.mb-0 En el diseño de las mecánicas del videojuego es necesario crear interacciones con el entorno, es en este punto donde los eventos ocurridos por condiciones físicas permiten a los jugadores recoger ítems de los niveles de juego, sufrir daño por pasar sobre zonas no permitidas, etc.
    p Los motores de videojuegos permiten simular los comportamientos físicos del entorno real haciendo uso de diferentes componentes como rigibodies, materiales físicos, colisionadores etc., permitiendo que las mecánicas sean dinámicas y parecidas a la realidad.
    .row.mt-4
      .col-2
        .row.align-items-center
          .col-3
            img(src='@/assets/curso/tema1/ico.svg', alt='Texto que describa la imagen')
          .col-9
            h4.mb-0 Triggers    
    p.mt-4 Los triggers son eventos que ocurren cuando los objetos de videojuego se entrelazan entre sí como se observa en la figura.
    .row.justify-content-center.mt-5
      .col-lg-10
        .titulo-sexto.color-acento-contenido
          h5 Figura 10
          span   Trigger entre gameobjects
        img(src='@/assets/curso/tema3/2.png', alt='Texto que describa la imagen')   
    .row.mt-4
      .col-2
        .row.align-items-center
          .col-3
            img(src='@/assets/curso/tema1/ico.svg', alt='Texto que describa la imagen')
          .col-9
            h4.mb-0 Collision
    p.mt-4 La colisión es un evento que ocurre cuando dos gameobjects se tocan entre sí, este evento es muy utilizado para provocar daño a los enemigos en un videojuego.    
    .row.justify-content-center.mt-5
      .col-lg-10
        .titulo-sexto.color-acento-contenido
          h5 Figura 11
          span   Collision
        img(src='@/assets/curso/tema3/3.png', alt='Texto que describa la imagen')
    p.mt-4 Los tipos de colliders son:
    .row.mb-5
      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/1.svg' alt='AvatarTop')

          .tarjeta.color-acento-contenido
            .p-4
              h2.text-center Sphere Collider
              p.text-center Este tipo de collider es muy usado en formas redondas.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/2.svg' alt='AvatarTop')

          .tarjeta.color-acento-contenido
            .p-4
              h2.text-center Box Collider
              p.text-center Es empleado en formas cubicas, edificios, carretera, etc.

      .col-md-6.col-lg.mb-5.mb-lg-0
        .tarjeta-avatar
          img(src='@/assets/curso/tema3/3.svg' alt='AvatarTop')

          .tarjeta.color-acento-contenido
            .p-4
              h2.text-center Capsule Collider
              p.text-center Utilizado en los personajes para crear zonas de daño; es muy utilizado en los troncos de los árboles.
    p.mt-3 En el siguiente video se estudian las físicas y colisiones en el motor de desarrollo.
    .video
      iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.mt-4
      .col-2
        .row.align-items-center
          .col-3
            img(src='@/assets/curso/tema1/ico.svg', alt='Texto que describa la imagen')
          .col-9
            h4.mb-0 OnControllerHit
    p.mt-3 Este tipo de colisión es característico en los personajes de los videojuegos, ya que permite detectar cuando el jugador recoge elementos del nivel de juego.
    .row.justify-content-center.mt-5
      .col-lg-4
        .titulo-sexto.color-acento-contenido
          h5 Figura 12
          span  Character controller
        img(src='@/assets/curso/tema3/4.png', alt='Texto que describa la imagen')         
    p.mt-4 A través de los siguientes videos se explicará cómo controlar un personaje y aplicar animaciones:
    h4.text-center.mt-4 Character controller para controlar el movimiento de un personaje.
    .video
      iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    h4.text-center.mt-4 Colisión con otros objetos de la escena.
    .video
      iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
      h4.text-center.mt-4 Generación de cámara de seguimiento al personaje.
    .video
      iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.justify-content-center.mt-5
      .col-lg-8
        .tarjeta.color-primario.p-3.mb-5
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema2/z.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Material complementario Unity Learn
                  p.text-small Para ampliar el tema sobre la programación de eventos disparadores e interacción con el entorno, consultar en el material complementario la página Unity Learn el tema de Catapult Physics; Forces, and Energy.
                .col-sm-auto
                  a.boton.color-acento-botones(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Enlace web
                    i.fas.fa-file-download                        
</template>

<script>
export default {
  name: 'Tema3',
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
