<template>
  <div>
    <app-navbar />
    <app-body />
  </div>
</template>

<script>
import AppNavbar from "./components/AppNavbar";
import AppBody from "./components/AppBody";

export default {
  name: "App",
  components: {
    AppNavbar,
    AppBody,
  },
};
</script>

<style>

</style>
