<template>
  <div class="services">
    <!-- Page Content -->
    <b-container>
      <h1 class="mt-4 mb-3">Services
        <small>Subheading</small>
      </h1>

      <!-- Page Heading/Breadcrumbs -->
      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Services</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Image Header -->
      <img class="img-fluid rounded mb-4" src="http://placehold.it/1200x300" alt="">

      <!-- Marketing Icons Section -->
      <b-card-group deck class="mb-4">
        <b-card header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h4 class="mb-0">Card Title</h4>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Learn More</b-button>
          </template>
        </b-card>

        <b-card header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h4 class="mb-0">Card Title</h4>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ipsam eos, nam perspiciatis natus commodi similique totam consectetur praesentium molestiae atque exercitationem ut consequuntur, sed eveniet, magni nostrum sint fuga.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Learn More</b-button>
          </template>
        </b-card>

        <b-card header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h4 class="mb-0">Card Title</h4>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Learn More</b-button>
          </template>
        </b-card>

      </b-card-group>
    </b-container>
  </div>
</template>
