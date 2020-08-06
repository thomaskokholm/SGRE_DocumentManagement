<template>
  <div class="DocumentManagement DocumentLibraryList">
    Document Library List goes here: {{cardView}}
    <div v-if="cardView">
      <div class="row">
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
        <div class="col-sm-12 col-md-6 col-lg-4 col-xl-3">
          <div class="card">
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
    <div class="table-responsive" v-else>
      <table class="table table-sm">
        <thead>
          <tr>
            <th>&nbsp;</th>
            <th scope="col">Title</th>
            <th scope="col">Document Type</th>
            <th scope="col">Language</th>
            <th scope="col">Version</th>
            <th scope="col">Year</th>
            <th scope="col">Month</th>
            <th scope="col">Modified</th>
            <th scope="col">Created</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>&mdash;</td>
            <td>HSE Document Title</td>
            <td>Safety Alert</td>
            <td>English</td>
            <td>1.0</td>
            <td>2020</td>
            <td>Jan</td>
            <td>June 20, 2020</td>
            <td>Jan 1, 2020</td>
          </tr>
          <tr>
            <td>&mdash;</td>
            <td>HSE Document Title</td>
            <td>Safety Alert</td>
            <td>Spainish</td>
            <td>1.0</td>
            <td>2020</td>
            <td>Jan</td>
            <td>June 20, 2020</td>
            <td>Jan 1, 2020</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "DocumentLibraryList",
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
