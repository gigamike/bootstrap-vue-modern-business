<template>
  <div class="404">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">404
        <small>Page Not Found</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>404</b-breadcrumb-item>
      </b-breadcrumb>

      <b-jumbotron>
        <h1 class="display-1">404</h1>
        <p>The page you're looking for could not be found. Here are some helpful links to get you back on track:</p>
        <ul>
          <li>
            <router-link :to="{ name: 'Home'}">Home</router-link>
          </li>
          <li>
            <router-link :to="{ name: 'About'}">About</router-link>
          </li>
          <li>
            <router-link :to="{ name: 'Services'}">Services</router-link>
          </li>
          <li>
            <router-link :to="{ name: 'Contact'}">Contact</router-link>
          </li>
          <li>
            Portfolio
            <ul>
              <li>
                <router-link :to="{ name: 'Portfolio-1-col'}">1 Column Portfolio</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Portfolio-2-col'}">2 Column Portfolio</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Portfolio-3-col'}">3 Column Portfolio</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Portfolio-4-col'}">4 Column Portfolio</router-link>
              </li>
            </ul>
          </li>
          <li>
            Blog
            <ul>
              <li>
                <router-link :to="{ name: 'Blog-home-1'}">Blog Home 1</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Blog-home-2'}">Blog Home 2</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Blog-post'}">Blog Post</router-link>
              </li>
            </ul>
          </li>
          <li>
            Other Pages
            <ul>
              <li>
                <router-link :to="{ name: 'Full-width'}">Full Width Page</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Sidebar'}">Sidebar Page</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'FAQ'}">FAQ</router-link>
              </li>
              <li>
                <router-link :to="{ name: '404'}">404 Page</router-link>
              </li>
              <li>
                <router-link :to="{ name: 'Pricing'}">Pricing Table</router-link>
              </li>
            </ul>
          </li>
        </ul>
      </b-jumbotron>

    </b-container>
  </div>
</template>
