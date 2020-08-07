<template>
  <div class="DocumentManagement DocumentLibraryList">
    <document-library-card v-if="cardView"></document-library-card>
    <document-library-table v-else></document-library-table>
  </div>
</template>

<script>
import DocumentLibraryCard from "./DocumentLibraryCard";
import DocumentLibraryTable from "./DocumentLibraryTable";
export default {
  name: "DocumentLibraryList",
  components: {
    DocumentLibraryCard,
    DocumentLibraryTable
  },
  props: {
    cardView: {
      type: Boolean,
      default: false,
      required: false
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.table th {
  border-top-color: transparent;
}
</style>
