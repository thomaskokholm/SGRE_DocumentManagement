<template>
  <div class="DocumentManagement DocumentLibraryCard">
    <div class="row">
      <div class="col-sm-6 col-md-6 col-lg-4 col-xl-3" v-for="index in 5" :key="index">
        <div class="card mb-4">
          <img class="card-img-top bg-light" src="https://source.unsplash.com/random/320x250">
          <div class="card-body">
            <h5 class="card-title">HSE Document Title</h5>
            <p class="card-text">June 20, 2020</p>
            <p class="card-text">
              <small class="text-muted">ENGLISH</small>
              <small class="text-muted float-right">v 1.0</small>
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
