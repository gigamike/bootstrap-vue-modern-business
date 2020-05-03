<template>
  <div class="portfolio-1-col">
    <b-container>
      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Portfolio 1
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Portfolio 1</b-breadcrumb-item>
      </b-breadcrumb>

      <div
        id="my-portfolio"
        v-for="item in lists" :key="item.id"
        :per-page="perPage"
        :current-page="currentPage"
      >
          <b-row>
            <b-col cols="7" md="7">
              <a href="#">
                <img class="img-fluid rounded mb-3 mb-md-0" src="http://placehold.it/700x300" alt="">
              </a>
            </b-col>
            <b-col cols="5" md="5">
              <h3>{{ item.title }}</h3>
              <p>{{ item.body }}</p>
              <a class="btn btn-primary" href="#">View Project
                <span class="glyphicon glyphicon-chevron-right"></span>
              </a>
            </b-col>
          </b-row>
        <!-- /.row -->

        <hr>
    </div>

      <!-- Pagination -->
      <div class="overflow-auto">
         <b-pagination
          class="justify-content-center"
           v-model="currentPage"
           :total-rows="rows"
           :per-page="perPage"
           aria-controls="my-portfolio"
         ></b-pagination>
       </div>
       
    </b-container>
    <!-- /.container -->
  </div>
</template>

<script>
  export default {
    data() {
      return {
        perPage: 4,
        currentPage: 1,
        items: [
          { id: 1, title: 'Project One', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 2, title: 'Project Two', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
          { id: 3, title: 'Project Three', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 4, title: 'Project Four', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 5, title: 'Project Five', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 6, title: 'Project Six', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
          { id: 7, title: 'Project Seven', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 8, title: 'Project Eight', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 9, title: 'Project Nine', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' }
        ]
      }
    },
    computed: {
      lists () {
        return this.items.slice(
          (this.currentPage - 1) * this.perPage,
          this.currentPage * this.perPage
        )
      },
      rows() {
        return this.items.length
      }
    }
  }
</script>
