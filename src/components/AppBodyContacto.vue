<template>
  <div class="container mb-5">
    <h2 class="text-center mb-4">Contacto</h2>
    <div class="d-grid gap-2 col-lg-5 col-md-6 mx-auto">
      <a
        href="https://api.whatsapp.com/send?phone=522381185749"
        class="btn btn-outline-success btn-lg"
        type="button"
        target="_blank"
      >
        <i class="fab fa-whatsapp"></i> WhatsApp
      </a>
      <a
        href="https://t.me/DaniTec1"
        class="btn btn-outline-primary btn-lg"
        type="button"
        target="_blank"
      >
        <i class="fab fa-telegram-plane"></i> Telegram
      </a>
      <a
        href="https://www.facebook.com/DaniTec1.github.io"
        class="btn btn-outline-primary btn-lg"
        type="button"
        target="_blank"
      >
        <i class="fab fa-facebook-f"></i> Facebook
      </a>
      <button
        id="share-btn"
        class="btn btn-outline-danger btn-lg"
        @click="compartir"
        hidden
      >
        <i class="fas fa-share-alt"></i> Compartir
      </button>
    </div>
    <div class="card mt-3">
      <div class="card-body d-flex justify-content-center">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1892.5110365892472!2d-97.3819300164325!3d18.437306897688718!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85c5bcf1cb88fbed%3A0xf3e6263e5f82b4e3!2sCalle%20Diego%20Rivera%20137%2C%20Cultural%2C%2075795%20Tehuac%C3%A1n%2C%20Pue.!5e0!3m2!1ses-419!2smx!4v1618725538561!5m2!1ses-419!2smx"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </div>
    </div>
    <div class="container"></div>
  </div>
</template>

<script>

const d = document,
  n = navigator,
  ua = n.userAgent;
const isMobile = {
  android: () => ua.match(/android/i),
  ios: () => ua.match(/iphone|ipad|ipod/i),
  windows: () => ua.match(/windows phone/i),
  any: function () {
    return this.android() || this.ios() || this.windows();
  },
};

export default {
  methods: {
    compartir() {
      if (navigator.share) {
        n.share({
          title: "DaniTec",
          url: "https://danitec1.github.io/",
          text: "Servicio Tecnico de Computadoras\n",
        });
      } else {
        console.log("Error");
      }
    },
    comprobar() {
      if (isMobile.any()) {
        let btn = document.getElementById("share-btn");
        btn.removeAttribute("hidden");
      }
    },
  },
  mounted() {
    this.comprobar();
  },
};
</script>

<style>
iframe {
  width: 100%;
  height: 400px;
}
</style>