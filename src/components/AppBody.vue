<template>
  <div class="container">
    <app-body-carousel />
    <app-body-descripcion />
    <app-body-servicios />
    <app-body-contacto />
  </div>
</template>

<script>
import AppBodyCarousel from './AppBodyCarousel.vue';
import AppBodyDescripcion from './AppBodyDescripcion.vue';
import AppBodyServicios from './AppBodyServicios.vue';
import AppBodyContacto from './AppBodyContacto.vue';

export default {
  name: "App",
  components: {
    AppBodyCarousel,
    AppBodyDescripcion,
    AppBodyServicios,
    AppBodyContacto
  },
};
</script>

<style>

</style>
