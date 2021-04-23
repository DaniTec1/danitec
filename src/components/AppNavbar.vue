<template>
  <nav
    id="navbar-example2"
    class="navbar navbar-expand-lg navbar-dark"
    style="background-color: #6610f2"
  >
    <div class="container">
      <a class="navbar-brand" href="">
        <i class="fas fa-desktop"></i> DaniTec</a
      >
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link text-light" href="#saludo">
              <i class="fab fa-angellist"></i> Saludo</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#servicios">
              <i class="fas fa-tasks"></i> Servicios</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link text-light" href="#contacto">
              <i class="fas fa-user-circle"></i> Contacto</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style>
/* class="navbar navbar-dark" style="background-color: #6610f2;" 
  class="navbar navbar-light bg-light px-3"
*/
</style>
