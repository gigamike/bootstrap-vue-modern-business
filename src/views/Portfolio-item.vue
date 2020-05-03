<template>
  <div class="portfolio-item">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Portfolio Item
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Portfolio Item</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Portfolio Item Row -->
      <b-row>
        <b-col cols="8" md="8" class="mt-1">
          <img class="img-fluid" src="http://placehold.it/750x500" alt="">
        </b-col>
        <b-col cols="4" md="4" class="mt-1 mb-4">
          <h3 class="my-3">Project Description</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae. Sed dui lorem, adipiscing in adipiscing et, interdum nec metus. Mauris ultricies, justo eu convallis placerat, felis enim.</p>
          <h3 class="my-3">Project Details</h3>
          <ul>
            <li>Lorem Ipsum</li>
            <li>Dolor Sit Amet</li>
            <li>Consectetur</li>
            <li>Adipiscing Elit</li>
          </ul>
        </b-col>
      </b-row>
      <!-- /.row -->

      <!-- Related Projects Row -->
      <h3 class="my-4">Related Projects</h3>

      <b-row>
        <b-col cols="3" md="3" sm="6" class="mt-1 mb-4">
          <a href="#">
            <img class="img-fluid" src="http://placehold.it/500x300" alt="">
          </a>
        </b-col>
        <b-col cols="3" md="3" sm="6" class="mt-1 mb-4">
          <a href="#">
            <img class="img-fluid" src="http://placehold.it/500x300" alt="">
          </a>
        </b-col>
        <b-col cols="3" md="3" sm="6" class="mt-1 mb-4">
          <a href="#">
            <img class="img-fluid" src="http://placehold.it/500x300" alt="">
          </a>
        </b-col>
        <b-col cols="3" md="3" sm="6" class="mt-1 mb-4">
          <a href="#">
            <img class="img-fluid" src="http://placehold.it/500x300" alt="">
          </a>
        </b-col>
      </b-row>

    </b-container>
  </div>
</template>
