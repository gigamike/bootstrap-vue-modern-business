<template>
  <div class="Blog-post">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Post Title
        <small>by
          <a href="#">Start Bootstrap</a>
        </small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Blog Home 2</b-breadcrumb-item>
      </b-breadcrumb>

      <b-row>
        <!-- Post Content Column -->
        <b-col cols="8" lg="8" class="mt-1 mb-4">
          <!-- Preview Image -->
          <img class="img-fluid rounded" src="http://placehold.it/900x300" alt="">

          <hr>

          <!-- Date/Time -->
          <p>Posted on January 1, 2017 at 12:00 PM</p>

          <hr>

          <!-- Post Content -->
          <p class="lead">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus, vero, obcaecati, aut, error quam sapiente nemo saepe quibusdam sit excepturi nam quia corporis eligendi eos magni recusandae laborum minus inventore?</p>

          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, tenetur natus doloremque laborum quos iste ipsum rerum obcaecati impedit odit illo dolorum ab tempora nihil dicta earum fugiat. Temporibus, voluptatibus.</p>

          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos, doloribus, dolorem iusto blanditiis unde eius illum consequuntur neque dicta incidunt ullam ea hic porro optio ratione repellat perspiciatis. Enim, iure!</p>

          <blockquote class="blockquote">
            <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
            <footer class="blockquote-footer">Someone famous in
              <cite title="Source Title">Source Title</cite>
            </footer>
          </blockquote>

          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error, nostrum, aliquid, animi, ut quas placeat totam sunt tempora commodi nihil ullam alias modi dicta saepe minima ab quo voluptatem obcaecati?</p>

          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum, dolor quis. Sunt, ut, explicabo, aliquam tenetur ratione tempore quidem voluptates cupiditate voluptas illo saepe quaerat numquam recusandae? Qui, necessitatibus, est!</p>

          <hr>

          <!-- Comments Form -->
          <b-card header-tag="header" class="my-4">
            <template v-slot:header>
              <h5 class="mb-0">Leave a Comment:</h5>
            </template>
            <b-card-text>
              <b-form-textarea
                    id="textarea"
                    v-model="text"
                    placeholder="Enter something..."
                    rows="3"
                  ></b-form-textarea>
              <b-button class="mt-3" type="submit" variant="primary">Submit</b-button>
            </b-card-text>
          </b-card>

          <!-- Single Comment -->
          <b-media class="mb-3">
            <template v-slot:aside>
              <b-img class="rounded-circle" blank blank-color="#ccc" width="64" alt="placeholder"></b-img>
            </template>

            <h5 class="mt-0">Commenter Name</h5>
            <p>
              Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
            </p>
          </b-media>

          <!-- Comment with nested comments -->
          <b-media class="mb-3">
            <template v-slot:aside>
              <b-img class="rounded-circle" blank blank-color="#ccc" width="64" alt="placeholder"></b-img>
            </template>

            <h5 class="mt-0">Commenter Name</h5>
            <p>
              Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
            </p>

            <b-media>
              <template v-slot:aside>
                <b-img class="rounded-circle" blank blank-color="#ccc" width="64" alt="placeholder"></b-img>
              </template>

              <h5 class="mt-0">Commenter Name</h5>
              <p class="mb-0">
                Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
              </p>
            </b-media>

            <b-media>
              <template v-slot:aside>
                <b-img class="rounded-circle" blank blank-color="#ccc" width="64" alt="placeholder"></b-img>
              </template>

              <h5 class="mt-0">Commenter Name</h5>
              <p class="mb-0">
                Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
              </p>
            </b-media>
          </b-media>
        </b-col>

        <!-- Sidebar Widgets Column -->
        <b-col cols="4" md="4" class="mt-1 mb-4">
          <!-- Search Widget -->
          <b-card header-tag="header">
            <template v-slot:header>
              <h5 class="mb-0">Search</h5>
            </template>
            <b-card-text>
              <b-input-group>
                <b-form-input type="text" placeholder="Search for..."></b-form-input>
                <b-input-group-append>
                  <b-button>Go!</b-button>
                </b-input-group-append>
              </b-input-group>
            </b-card-text>
          </b-card>

          <!-- Categories Widget -->
          <b-card header-tag="header" class="mt-4 mb-4">
            <template v-slot:header>
              <h5 class="mb-0">Categories</h5>
            </template>
            <b-card-text>
              <b-row>
                <b-col cols="6" lg="6">
                  <ul class="list-unstyled mb-0">
                    <li>
                      <a href="#">Web Design</a>
                    </li>
                    <li>
                      <a href="#">HTML</a>
                    </li>
                    <li>
                      <a href="#">Freebies</a>
                    </li>
                  </ul>
                </b-col>
                <b-col cols="6" lg="6">
                  <ul class="list-unstyled mb-0">
                    <li>
                      <a href="#">JavaScript</a>
                    </li>
                    <li>
                      <a href="#">CSS</a>
                    </li>
                    <li>
                      <a href="#">Tutorials</a>
                    </li>
                  </ul>
                </b-col>
              </b-row>
            </b-card-text>
          </b-card>

          <!-- Side Widget -->
          <b-card header-tag="header" class="mt-4 mb-4">
            <template v-slot:header>
              <h5 class="mb-0">Side Widget</h5>
            </template>
            <b-card-text>
              You can put anything you want inside of these side widgets. They are easy to use, and feature the new Bootstrap 4 card containers!
            </b-card-text>
          </b-card>
        </b-col>
      </b-row>

    </b-container>
  </div>
</template>
