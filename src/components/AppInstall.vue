<template>
  <div
    class="modal fade"
    id="modal"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content">
        <!-- <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Atención</h5>
        </div> -->
        <div class="modal-body">
          <p class="h3">¿Le gustaría llevarse mi tarjeta?</p>
        </div>
        <div class="modal-footer">
          <button
            type="button"
            class="btn btn-outline-danger"
            data-bs-dismiss="modal"
            @click="dismiss"
          >
            No Gracias
          </button>
          <button
            data-bs-dismiss="modal"
            type="button"
            class="btn btn-success"
            @click="install"
          >
            <i class="fas fa-download"></i>
            Si
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppInstall",
  data() {
    return {
      deferredPrompt: null,
    };
  },
  methods: {
    async dismiss() {
      this.deferredPrompt = null;
    },
    async install() {
      this.deferredPrompt.prompt();
    },
    isInstall() {
      const myModal = new bootstrap.Modal(document.getElementById("modal"));
      if (window.matchMedia("(display-mode: standalone)").matches) {
      } else {
        myModal.show();
      }
    },
    cerrar() {
      myModal.hide();
    },
  },
  created() {
    window.addEventListener("beforeinstallprompt", (e) => {
      e.preventDefault();
      // Stash the event so it can be triggered later.
      this.deferredPrompt = e;
    });
    window.addEventListener("appinstalled", () => {
      this.deferredPrompt = null;
    });
  },
  mounted() {
    window.onload = function() {
      setTimeout(this.isInstall, 20000);
    }
  },
};
</script>

<style>
</style>