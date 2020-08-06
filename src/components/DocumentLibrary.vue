<template>
  <div class="DocumentManagement DocumentLibrary">
    <div class="d-flex mb-3">
      <div class="flex-grow-1">
        <DocumentLibrarySearchbar></DocumentLibrarySearchbar>
      </div>
      <div class="bg-light border-top border-right border-bottom border-secondary p-2">List / Grid</div>
    </div>
    <div class="row">
      <div class="col-sm-12 col-md-5 col-lg-4">
        <DocumentLibraryFilters></DocumentLibraryFilters>
      </div>
      <div class="col-sm-12 col-md-7 col-lg-8">
        <DocumentLibraryList></DocumentLibraryList>
      </div>
    </div>
  </div>
</template>

<script>
import DocumentLibraryList from "./DocumentLibraryList";
import DocumentLibraryFilters from "./DocumentLibraryFilters";
import DocumentLibrarySearchbar from "./DocumentLibrarySearchbar";
export default {
  name: "DocumentLibrary",
  components: {
    DocumentLibraryList,
    DocumentLibraryFilters,
    DocumentLibrarySearchbar
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
