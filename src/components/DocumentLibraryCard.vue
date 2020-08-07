<template>
  <div class="DocumentManagement DocumentLibraryCard">
    <div class="row">
      <div class="col-sm-6 col-md-6 col-lg-4 col-xl-3" v-for="index in 5" :key="index">
        <div class="card w-100">
          <img class="card-img-top" alt>
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <p
              class="card-text"
            >This is a longer card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
            <p class="card-text">
              <small class="text-muted">Last updated 3 mins ago</small>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DocumentLibraryCard"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
