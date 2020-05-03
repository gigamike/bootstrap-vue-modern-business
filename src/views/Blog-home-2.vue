<template>
  <div class="blog-home-2">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Blog Home Two
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Blog Home 2</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Blog Post -->
      <b-card class="mt-1 mb-4"
        id="my-blog"
        v-for="item in lists" :key="item.id"
        :per-page="perPage"
        :current-page="currentPage"
      >
        <b-card-text>
          <b-row>
            <b-col cols="6" lg="6">
              <a href="#">
                <img class="img-fluid rounded" src="http://placehold.it/750x300" alt="">
              </a>
            </b-col>
            <b-col cols="6" lg="6">
              <h2 class="card-title">Post Title</h2>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis aliquid atque, nulla? Quos cum ex quis soluta, a laboriosam. Dicta expedita corporis animi vero voluptate voluptatibus possimus, veniam magni quis!</p>
              <a href="#" class="btn btn-primary">Read More &rarr;</a>
            </b-col>
          </b-row>
        </b-card-text>
        <template v-slot:footer>
          Posted on January 1, 2017 by
          <a href="#">Start Bootstrap</a>
        </template>
      </b-card>

      <!-- Pagination -->
      <div class="overflow-auto">
         <b-pagination
          class="justify-content-center mb-4"
           v-model="currentPage"
           :total-rows="rows"
           :per-page="perPage"
           aria-controls="my-blog"
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
        perPage: 3,
        currentPage: 1,
        items: [
          { id: 1, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis aliquid atque, nulla? Quos cum ex quis soluta, a laboriosam. Dicta expedita corporis animi vero voluptate voluptatibus possimus, veniam magni quis!' },
          { id: 2, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis aliquid atque, nulla? Quos cum ex quis soluta, a laboriosam. Dicta expedita corporis animi vero voluptate voluptatibus possimus, veniam magni quis!' },
          { id: 3, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis aliquid atque, nulla? Quos cum ex quis soluta, a laboriosam. Dicta expedita corporis animi vero voluptate voluptatibus possimus, veniam magni quis!' },
          { id: 4, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 5, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 6, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
          { id: 7, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 8, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 9, title: 'Post Title', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' }
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
