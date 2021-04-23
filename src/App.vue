<template>
  <div>
    <app-navbar />
    <app-body />
    <app-install />
  </div>
</template>

<script>
import AppNavbar from "./components/AppNavbar";
import AppBody from "./components/AppBody";
import AppInstall from "./components/AppInstall";

export default {
  name: "App",
  components: {
    AppNavbar,
    AppBody,
    AppInstall,
  },
};
</script>

<style>
</style>
