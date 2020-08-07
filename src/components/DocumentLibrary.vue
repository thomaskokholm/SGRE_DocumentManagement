<template>
  <div class="DocumentManagement DocumentLibrary">
    <div class="d-flex mb-3">
      <div class="flex-grow-1">
        <document-library-searchbar></document-library-searchbar>
      </div>
      <div class="bg-light border-top border-right border-bottom border-secondary">
        <button
          class="btn"
          v-on:click="setListView()"
          :class="!isCardView ? 'btn-secondary' : 'btn-light'"
        >List</button>
        <button
          class="btn"
          v-on:click="setCardView()"
          :class="isCardView ? 'btn-secondary' : 'btn-light'"
        >Card</button>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12 col-md-5 col-lg-4 col-xl-3">
        <document-library-filters></document-library-filters>
      </div>
      <div class="col-sm-12 col-md-7 col-lg-8 col-xl-9">
        <document-library-list :cardView="isCardView"></document-library-list>
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
