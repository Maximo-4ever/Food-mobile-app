<template>
  <TheNavbar />
  <RouterView />
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";
export default {
  components: { TheNavbar },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Poppins", sans-serif;
}
</style>
