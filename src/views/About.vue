<template>
  <div class="about">
    <b-container>
      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">About
        <small>Subheading</small>
      </h1>

      <ol class="breadcrumb">
        <li class="breadcrumb-item">
          <router-link :to="{name: 'Home'}">Home</router-link>
        </li>
        <li class="breadcrumb-item active">About</li>
      </ol>

      <!-- Intro Content -->
      <b-row>
        <b-col cols="6" lg="6">
          <img class="img-fluid rounded mb-4" src="http://placehold.it/750x450" alt="">
        </b-col>
        <b-col cols="6" lg="6">
          <h2>About Modern Business</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sed voluptate nihil eum consectetur similique? Consectetur, quod, incidunt, harum nisi dolores delectus reprehenderit voluptatem perferendis dicta dolorem non blanditiis ex fugiat.</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe, magni, aperiam vitae illum voluptatum aut sequi impedit non velit ab ea pariatur sint quidem corporis eveniet. Odit, temporibus reprehenderit dolorum!</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Et, consequuntur, modi mollitia corporis ipsa voluptate corrupti eum ratione ex ea praesentium quibusdam? Aut, in eum facere corrupti necessitatibus perspiciatis quis?</p>
        </b-col>
      </b-row>
      <!-- /.row -->

      <!-- Team Members -->
      <h2>Our Team</h2>

      <b-card-group deck class="mb-4 text-center">
        <b-card title="Team Member" footer-tag="footer" img-src="http://placehold.it/750x450">
          <b-card-text>
            <h6 class="card-subtitle mb-2 text-muted">Position</h6>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus aut mollitia eum ipsum fugiat odio officiis odit.</p>
          </b-card-text>
          <template v-slot:footer>
            <a href="#">name@example.com</a>
          </template>
        </b-card>

        <b-card title="Team Member" footer-tag="footer" img-src="http://placehold.it/750x450">
          <b-card-text>
            <h6 class="card-subtitle mb-2 text-muted">Position</h6>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus aut mollitia eum ipsum fugiat odio officiis odit.</p>
          </b-card-text>
          <template v-slot:footer>
            <a href="#">name@example.com</a>
          </template>
        </b-card>

        <b-card title="Team Member" footer-tag="footer" img-src="http://placehold.it/750x450">
          <b-card-text>
            <h6 class="card-subtitle mb-2 text-muted">Position</h6>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus aut mollitia eum ipsum fugiat odio officiis odit.</p>
          </b-card-text>
          <template v-slot:footer>
            <a href="#">name@example.com</a>
          </template>
        </b-card>
      </b-card-group>

      <!-- Our Customers -->
      <h2>Our Customers</h2>
      <b-row>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
        <b-col cols="2" lg="2" sm="2" class="mb-4">
          <img class="img-fluid" src="http://placehold.it/500x300" alt="">
        </b-col>
      </b-row>
      <!-- /.row -->
    </b-container>
  </div>
</template>
