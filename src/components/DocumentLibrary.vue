<template>
  <div class="DocumentManagement DocumentLibrary">
    <div class="d-flex mb-3">
      <div class="flex-grow-1">
        <DocumentLibrarySearchbar></DocumentLibrarySearchbar>
      </div>
      <div class="bg-light border-top border-right border-bottom border-secondary">
        <button class="btn btn-light" v-on:click="setListView()">List</button>
        <button class="btn btn-light" v-on:click="setCardView()">Card</button>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12 col-md-5 col-lg-4 col-xl-3">
        <DocumentLibraryFilters></DocumentLibraryFilters>
      </div>
      <div class="col-sm-12 col-md-7 col-lg-8 col-xl-9">
        <DocumentLibraryList :cardView="isCardView"></DocumentLibraryList>
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
  },
  data() {
    return {
      isCardView: false
    };
  },

  methods: {
    setCardView() {
      this.isCardView = true;
    },
    setListView() {
      this.isCardView = false;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
