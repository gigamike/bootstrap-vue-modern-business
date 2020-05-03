<template>
  <div id="app">
    <div>
      <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
        <b-container>
          <b-navbar-brand :to="{name: 'Home'}">Vue Bootstrap</b-navbar-brand>

          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

          <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav class="ml-auto">
            </b-navbar-nav>
            <b-navbar-nav>
              <b-nav-item :to="{name: 'About'}">About</b-nav-item>
              <b-nav-item :to="{name: 'Services'}">Services</b-nav-item>
              <b-nav-item :to="{name: 'Contact'}">Contact</b-nav-item>
              <b-nav-item-dropdown text="Portfolio" right>
                <b-dropdown-item :to="{name: 'Portfolio-1-col'}">1 Column Portfolio</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Portfolio-2-col'}">2 Column Portfolio</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Portfolio-3-col'}">3 Column Portfolio</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Portfolio-4-col'}">4 Column Portfolio</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Portfolio-item'}">Single Portfolio Item</b-dropdown-item>
              </b-nav-item-dropdown>
              <b-nav-item-dropdown text="Blog" right>
                <b-dropdown-item :to="{name: 'Blog-home-1'}">Blog Home 1</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Blog-home-2'}">Blog Home 2</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Blog-post'}">Blog Post</b-dropdown-item>
              </b-nav-item-dropdown>
              <b-nav-item-dropdown text="Other Pages" right>
                <b-dropdown-item :to="{name: 'Full-width'}">Full Width Page</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Sidebar'}">Sidebar Page</b-dropdown-item>
                <b-dropdown-item :to="{name: 'FAQ'}">FAQ</b-dropdown-item>
                <b-dropdown-item :to="{name: '404'}">404</b-dropdown-item>
                <b-dropdown-item :to="{name: 'Pricing'}">Pricing Table</b-dropdown-item>
              </b-nav-item-dropdown>
            </b-navbar-nav>
          </b-collapse>
        </b-container>
      </b-navbar>
    </div>

    <router-view />

    <!-- Footer -->
    <footer class="py-5 bg-dark">
      <div class="container">
        <p class="m-0 text-center text-white">Copyright &copy; Your Website 2019</p>
      </div>
      <!-- /.container -->
    </footer>
  </div>
</template>

<style>
body { padding-top: 60px; }
</style>
