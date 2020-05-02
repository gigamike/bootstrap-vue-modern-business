<template>
  <div class="home">
    <header>
      <b-carousel
        id="carousel-fade"
        style="text-shadow: 0px 0px 2px #000"
        fade
        indicators
        img-width="1024"
        img-height="500"
      >
        <b-carousel-slide
          caption="First slide"
          img-src="http://placehold.it/1900x500"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Second Slide"
          img-src="http://placehold.it/1900x500"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Third Slide"
          img-src="http://placehold.it/1900x500"
        ></b-carousel-slide>
      </b-carousel>
    </header>

    <b-container>
      <h1 class="my-4">Welcome to Modern Business</h1>

      <b-card-group deck>
        <b-card title="Title" header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h6 class="mb-0">Header Slot</h6>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Go somewhere</b-button>
          </template>
        </b-card>

        <b-card title="Title" header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h6 class="mb-0">Header Slot</h6>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Go somewhere</b-button>
          </template>
        </b-card>

        <b-card title="Title" header-tag="header" footer-tag="footer">
          <template v-slot:header>
            <h6 class="mb-0">Header Slot</h6>
          </template>
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
          <template v-slot:footer>
            <b-button href="#" variant="primary">Go somewhere</b-button>
          </template>
        </b-card>
      </b-card-group>

      <h2 class="my-4">Portfolio Heading</h2>

      <b-card-group deck>
        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>

        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>

        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>
      </b-card-group>

      <b-card-group deck class="my-4">
        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>

        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>

        <b-card title="Title" img-src="https://picsum.photos/600/300/?image=25" header-tag="header" footer-tag="footer">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</b-card-text>
        </b-card>
      </b-card-group>

      <b-row class="mb-4">
        <b-col>
          <h2>Modern Business Features</h2>
          <p>The Modern Business template by Start Bootstrap includes:</p>
          <ul>
            <li>
              <strong>Bootstrap v4</strong>
            </li>
            <li>Vue</li>
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
