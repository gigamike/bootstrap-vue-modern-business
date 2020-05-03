<template>
  <div class="pricing">
    <!-- Page Content -->
    <b-container>
      <h1 class="mt-4 mb-3">Pricing
        <small>Subheading</small>
      </h1>

      <!-- Page Heading/Breadcrumbs -->
      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Pricing</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Content Row -->
      <b-row>
        <b-col cols="4" lg="4" class="mb-4">
          <b-card no-body>
            <template v-slot:header>
              <h3 class="mb-0">Basic</h3>
            </template>

            <b-card-body>
              <b-card-text>
                <div class="display-4">$19.99</div>
                <div class="font-italic">per month</div>
              </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Cras justo odio</b-list-group-item>
              <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
              <b-list-group-item>Vestibulum at eros</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a href="#" class="btn btn-primary">Sign Up!</a>
            </b-card-body>

          </b-card>
        </b-col>
        <b-col cols="4" lg="4" class="mb-4">
          <b-card
            no-body
            header-bg-variant="primary"
            header-text-variant="white"
          >
            <template v-slot:header>
              <h3 class="mb-0">Plus</h3>
            </template>

            <b-card-body>
              <b-card-text>
                <div class="display-4">$39.99</div>
                <div class="font-italic">per month</div>
              </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Cras justo odio</b-list-group-item>
              <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
              <b-list-group-item>Vestibulum at eros</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a href="#" class="btn btn-primary">Sign Up!</a>
            </b-card-body>

          </b-card>
        </b-col>
        <b-col cols="4" lg="4" class="mb-4">
          <b-card no-body>
            <template v-slot:header>
              <h3 class="mb-0">Ultra</h3>
            </template>

            <b-card-body>
              <b-card-text>
                <div class="display-4">$159.99</div>
                <div class="font-italic">per month</div>
              </b-card-text>
            </b-card-body>

            <b-list-group flush>
              <b-list-group-item>Cras justo odio</b-list-group-item>
              <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
              <b-list-group-item>Vestibulum at eros</b-list-group-item>
            </b-list-group>

            <b-card-body>
              <a href="#" class="btn btn-primary">Sign Up!</a>
            </b-card-body>

          </b-card>
        </b-col>
      </b-row>
      <!-- /.row -->

    </b-container>
    <!-- /.container -->
  </div>
</template>
