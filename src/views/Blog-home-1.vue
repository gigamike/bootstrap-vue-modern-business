<template>
  <div class="blog-home-1">
    <!-- Page Content -->
    <b-container>
      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Blog Home One
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Blog Home 1</b-breadcrumb-item>
      </b-breadcrumb>

      <b-row>
        <b-col cols="8" md="8" class="mt-1 mb-4">
          <b-card
            header-tag="header"
            footer-tag="footer"
            img-src="http://placehold.it/750x300"
            id="my-blog"
            v-for="item in lists" :key="item.id"
            :per-page="perPage"
            :current-page="currentPage"
            class="mb-4"
          >
            <h2>{{ item.title }}</h2>
            <b-card-text>{{ item.body }}</b-card-text>
            <a href="#" class="btn btn-primary">Read More &rarr;</a>
            <template v-slot:footer>
              Posted on January 1, 2017 by
              <a href="#">Start Bootstrap</a>
            </template>
          </b-card>

          <!-- Pagination -->
          <div class="overflow-auto">
             <b-pagination
              class="justify-content-center"
               v-model="currentPage"
               :total-rows="rows"
               :per-page="perPage"
               aria-controls="my-blog"
             ></b-pagination>
           </div>
        </b-col>

        <!-- Sidebar Widgets Column -->
        <b-col cols="4" md="4" class="mt-1 mb-4">
          <!-- Search Widget -->
          <b-card header-tag="header">
            <template v-slot:header>
              <h5 class="mb-0">Search</h5>
            </template>
            <b-card-text>
              <b-input-group>
                <b-form-input type="text" placeholder="Search for..."></b-form-input>
                <b-input-group-append>
                  <b-button>Go!</b-button>
                </b-input-group-append>
              </b-input-group>
            </b-card-text>
          </b-card>

          <!-- Categories Widget -->
          <b-card header-tag="header" class="mt-4 mb-4">
            <template v-slot:header>
              <h5 class="mb-0">Categories</h5>
            </template>
            <b-card-text>
              <b-row>
                <b-col cols="6" lg="6">
                  <ul class="list-unstyled mb-0">
                    <li>
                      <a href="#">Web Design</a>
                    </li>
                    <li>
                      <a href="#">HTML</a>
                    </li>
                    <li>
                      <a href="#">Freebies</a>
                    </li>
                  </ul>
                </b-col>
                <b-col cols="6" lg="6">
                  <ul class="list-unstyled mb-0">
                    <li>
                      <a href="#">JavaScript</a>
                    </li>
                    <li>
                      <a href="#">CSS</a>
                    </li>
                    <li>
                      <a href="#">Tutorials</a>
                    </li>
                  </ul>
                </b-col>
              </b-row>
            </b-card-text>
          </b-card>

          <!-- Side Widget -->
          <b-card header-tag="header" class="mt-4 mb-4">
            <template v-slot:header>
              <h5 class="mb-0">Side Widget</h5>
            </template>
            <b-card-text>
              You can put anything you want inside of these side widgets. They are easy to use, and feature the new Bootstrap 4 card containers!
            </b-card-text>
          </b-card>
        </b-col>
      </b-row>
      <!-- /.row -->

    </b-container>
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
