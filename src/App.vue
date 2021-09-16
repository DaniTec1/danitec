<template>
  <div>
    <app-navbar />
    <app-body />
    <app-install />
    <app-footer />
  </div>
</template>

<script>
import AppNavbar from "./components/AppNavbar";
import AppBody from "./components/AppBody";
import AppInstall from "./components/AppInstall";
import AppFooter from "./components/AppFooter";

export default {
  name: "App",
  components: {
    AppNavbar,
    AppBody,
    AppInstall,
    AppFooter,
  },
};
</script>

<style>
</style>
