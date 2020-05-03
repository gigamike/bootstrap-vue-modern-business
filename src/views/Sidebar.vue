<template>
  <div class="sidebar">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Sidebar Page
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>About</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Content Row -->
      <b-row>
        <!-- Sidebar Column -->
        <b-col cols="3" lg="3" class="mb-4">
          <div class="list-group">
            <a href="index.html" class="list-group-item">Home</a>
            <a href="about.html" class="list-group-item">About</a>
            <a href="services.html" class="list-group-item">Services</a>
            <a href="contact.html" class="list-group-item">Contact</a>
            <a href="portfolio-1-col.html" class="list-group-item">1 Column Portfolio</a>
            <a href="portfolio-2-col.html" class="list-group-item">2 Column Portfolio</a>
            <a href="portfolio-3-col.html" class="list-group-item">3 Column Portfolio</a>
            <a href="portfolio-4-col.html" class="list-group-item">4 Column Portfolio</a>
            <a href="portfolio-item.html" class="list-group-item">Single Portfolio Item</a>
            <a href="blog-home-1.html" class="list-group-item">Blog Home 1</a>
            <a href="blog-home-2.html" class="list-group-item">Blog Home 2</a>
            <a href="blog-post.html" class="list-group-item">Blog Post</a>
            <a href="full-width.html" class="list-group-item">Full Width Page</a>
            <a href="sidebar.html" class="list-group-item active">Sidebar Page</a>
            <a href="faq.html" class="list-group-item">FAQ</a>
            <a href="404.html" class="list-group-item">404</a>
            <a href="pricing.html" class="list-group-item">Pricing Table</a>
          </div>
        </b-col>
        <!-- Content Column -->
        <b-col cols="9" lg="9" class="mb-4">
          <h2>Section Heading</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta, et temporibus, facere perferendis veniam beatae non debitis, numquam blanditiis necessitatibus vel mollitia dolorum laudantium, voluptate dolores iure maxime ducimus fugit.</p>
        </b-col>
      </b-row>

    </b-container>
  </div>
</template>
