<template>
  <div class="portfolio-2-col">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Portfolio 2
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Portfolio 2</b-breadcrumb-item>
      </b-breadcrumb>

      <b-row>
        <b-col cols="6" md="6" class="mt-1 mb-4"
          id="my-portfolio"
          v-for="item in lists" :key="item.id"
          :per-page="perPage"
          :current-page="currentPage">
          <b-card
            header-tag="header"
            img-src="http://placehold.it/700x400"
            class="h-100"
          >
            <b-link to="/">
              <h4>{{ item.title }}</h4>
            </b-link>
            <b-card-text>{{ item.body }}</b-card-text>
          </b-card>
        </b-col>
      </b-row>

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
        perPage: 6,
        currentPage: 1,
        items: [
          { id: 1, title: 'Project One', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.' },
          { id: 2, title: 'Project Two', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit aliquam aperiam nulla perferendis dolor nobis numquam, rem expedita, aliquid optio, alias illum eaque. Non magni, voluptates quae, necessitatibus unde temporibus.' },
          { id: 3, title: 'Project Three', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.' },
          { id: 4, title: 'Project Four', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit aliquam aperiam nulla perferendis dolor nobis numquam, rem expedita, aliquid optio, alias illum eaque. Non magni, voluptates quae, necessitatibus unde temporibus.' },
          { id: 5, title: 'Project Five', body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.' },
          { id: 6, title: 'Project Six', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit aliquam aperiam nulla perferendis dolor nobis numquam, rem expedita, aliquid optio, alias illum eaque. Non magni, voluptates quae, necessitatibus unde temporibus.' },
          { id: 7, title: 'Project Seven', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 8, title: 'Project Eight', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 9, title: 'Project Nine', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 10, title: 'Project Ten', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 11, title: 'Project Eleven', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
          { id: 12, title: 'Project Twelve', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 13, title: 'Project Thirteen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 14, title: 'Project Fourteen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
          { id: 15, title: 'Project Fifteen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis, temporibus, dolores, at, praesentium ut unde repudiandae voluptatum sit ab debitis suscipit fugiat natus velit excepturi amet commodi deleniti alias possimus!' },
          { id: 16, title: 'Project Sixteen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo, quidem, consectetur, officia rem officiis illum aliquam perspiciatis aspernatur quod modi hic nemo qui soluta aut eius fugit quam in suscipit?' },
          { id: 17, title: 'Project Seventeen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium veniam exercitationem expedita laborum at voluptate. Labore, voluptates totam at aut nemo deserunt rem magni pariatur quos perspiciatis atque eveniet unde.' },
          { id: 18, title: 'Project Eighteen', body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, odit velit cumque vero doloremque repellendus distinctio maiores rem expedita a nam vitae modi quidem similique ducimus! Velit, esse totam tempore.' },
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
