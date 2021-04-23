<template>
  <div class="container">
    <app-body-carousel />
    <div data-bs-spy="scroll" data-bs-target="#navbar-example2" data-bs-offset="0" tabindex="0">
      <app-body-descripcion id="saludo" />
      <app-body-servicios id="servicios" />
      <app-body-contacto id="contacto" />
    </div>
  </div>
</template>

<script>
import AppBodyCarousel from "./AppBodyCarousel.vue";
import AppBodyDescripcion from "./AppBodyDescripcion.vue";
import AppBodyServicios from "./AppBodyServicios.vue";
import AppBodyContacto from "./AppBodyContacto.vue";

export default {
  name: "App",
  components: {
    AppBodyCarousel,
    AppBodyDescripcion,
    AppBodyServicios,
    AppBodyContacto,
  },
};
</script>

<style>
</style>
