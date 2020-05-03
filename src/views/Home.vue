<template>
  <div class="home">
    <header>
      <b-carousel
        id="carousel-fade"
        fade
        indicators
        img-width="1024"
        img-height="660"
        :interval="4000"
        controls
      >
        <b-carousel-slide
          caption="First slide"
          img-src="http://placehold.it/1900x660"
        >
          <p>This is a description for the first slide.</p>
        </b-carousel-slide>
        <b-carousel-slide
          caption="Second Slide"
          img-src="http://placehold.it/1900x660"
        >
          <p>This is a description for the second slide.</p>
        </b-carousel-slide>
        <b-carousel-slide
          caption="Third Slide"
          img-src="http://placehold.it/1900x660"
        >
          <p>This is a description for the third slide.</p>
        </b-carousel-slide>
      </b-carousel>
    </header>

    <b-container>
      <h1 class="my-4">Welcome to Modern Business</h1>

      <!-- Marketing Icons Section -->
      <b-card-group deck class="h-100">
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

      <!-- Portfolio Section -->
      <h2 class="my-4">Portfolio Heading</h2>

      <b-card-group deck>
        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project One</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet numquam aspernatur eum quasi sapiente nesciunt? Voluptatibus sit, repellat sequi itaque deserunt, dolores in, nesciunt, illum tempora ex quae? Nihil, dolorem!</b-card-text>
        </b-card>

        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project Two</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.</b-card-text>
        </b-card>

        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project One</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos quisquam, error quod sed cumque, odio distinctio velit nostrum temporibus necessitatibus et facere atque iure perspiciatis mollitia recusandae vero vel quam!</b-card-text>
        </b-card>
      </b-card-group>

      <b-card-group deck class="my-4">
        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project One</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.</b-card-text>
        </b-card>

        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project One</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam viverra euismod odio, gravida pellentesque urna varius vitae.</b-card-text>
        </b-card>

        <b-card img-src="http://placehold.it/700x400">
          <b-card-title><a href="#">Project One</a></b-card-title>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Itaque earum nostrum suscipit ducimus nihil provident, perferendis rem illo, voluptate atque, sit eius in voluptates, nemo repellat fugiat excepturi! Nemo, esse.</b-card-text>
        </b-card>
      </b-card-group>

      <b-row class="mb-3">
        <b-col>
          <h2>Modern Business Features</h2>
          <p>The Modern Business template by Start Bootstrap includes:</p>
          <ul>
            <li>
              <strong>Bootstrap v4</strong>
            </li>
            <li>Vue</li>
            <li>Webpack</li>
            <li>Working contact form with validation</li>
            <li>Unstyled page elements for easy customization</li>
          </ul>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis, omnis doloremque non cum id reprehenderit, quisquam totam aspernatur tempora minima unde aliquid ea culpa sunt. Reiciendis quia dolorum ducimus unde.</p>
        </b-col>
        <b-col>
          <img class="img-fluid rounded" src="http://placehold.it/700x450" alt="">
        </b-col>
      </b-row>

      <hr>

      <!-- Call to Action Section -->
      <b-row class="mb-4">
        <b-col cols="8">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias, expedita, saepe, vero rerum deleniti beatae veniam harum neque nemo praesentium cum alias asperiores commodi.</p>
        </b-col>
        <b-col cols="4">
          <a class="btn btn-lg btn-secondary btn-block" href="#">Call to Action</a>
        </b-col>
      </b-row>

    </b-container>


  </div>
</template>

<script>
// @ is an alias to /src

export default {

};
</script>
