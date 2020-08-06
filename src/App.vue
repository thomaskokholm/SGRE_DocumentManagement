<template>
  <div id="app" class="container-fluid mt-5">
    <DocumentLibrary></DocumentLibrary>
  </div>
</template>

<script>
import DocumentLibrary from "./components/DocumentLibrary";

export default {
  name: "App",
  components: {
    DocumentLibrary
  }
};
</script>

<style scoped>
.container-fluid {
  max-width: 1440px;
}
</style>
