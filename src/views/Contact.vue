<template>
  <div class="contact">
    <!-- Page Content -->
    <b-container>

      <!-- Page Heading/Breadcrumbs -->
      <h1 class="mt-4 mb-3">Contact
        <small>Subheading</small>
      </h1>

      <b-breadcrumb>
        <b-breadcrumb-item :to="{name: 'Home'}">
          Home
        </b-breadcrumb-item>
        <b-breadcrumb-item active>Contact</b-breadcrumb-item>
      </b-breadcrumb>

      <!-- Content Row -->
      <b-row>
        <!-- Map Column -->
        <b-col cols=8 lg="8" clas="mb-4">
          <!-- Embedded Google Map -->
          <iframe width="100%" height="400px" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://maps.google.com/maps?hl=en&amp;ie=UTF8&amp;ll=37.0625,-95.677068&amp;spn=56.506174,79.013672&amp;t=m&amp;z=4&amp;output=embed"></iframe>
        </b-col>
        <b-col cols=4 lg="4" clas="mb-4">
          <h3>Contact Details</h3>
          <p>
            3481 Melrose Place
            <br>Beverly Hills, CA 90210
            <br>
          </p>
          <p>
            <abbr title="Phone">P</abbr>: (123) 456-7890
          </p>
          <p>
            <abbr title="Email">E</abbr>:
            <a href="mailto:name@example.com">name@example.com
            </a>
          </p>
          <p>
            <abbr title="Hours">H</abbr>: Monday - Friday: 9:00 AM to 5:00 PM
          </p>
        </b-col>
      </b-row>
      <!-- /.row -->

      <!-- Contact Form -->
      <!-- In order to set the email address and subject line for the contact form go to the bin/contact_me.php file. -->
      <b-row>
        <b-col cols=8 lg="8" clas="mb-4">
          <h3>Send us a Message</h3>
          <b-form @submit="onSubmit" name="sentMessage" id="contactForm" novalidate>
            <b-form-group
              id="input-group-1"
              label="Full Name:"
              label-for="name"
            >
              <b-form-input
                id="name"
                v-model="form.name"
                type="text"
                required
                data-validation-required-message="Please enter your name."
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-2"
              label="Phone Number:"
              label-for="phone"
            >
              <b-form-input
                id="phone"
                v-model="form.name"
                type="text"
                required
                data-validation-required-message="Please enter your phone number."
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-3"
              label="Email Address:"
              label-for="email"
            >
              <b-form-input
                id="email"
                v-model="form.email"
                type="email"
                required
                data-validation-required-message="Please enter your email address."
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-4"
              label="Message:"
              label-for="message"
            >
              <b-form-textarea
                id="message"
                v-model="message"
                required data-validation-required-message="Please enter your message"
                maxlength="999"
                style="resize:none"
                rows="10"
                cols="100"
              ></b-form-textarea>
            </b-form-group>

            <div id="success"></div>
            <!-- For success/fail messages -->

            <b-form-group
            >
            <b-button type="submit" variant="primary" id="sendMessageButton">Send Message</b-button>
            </b-form-group>
          </b-form>
        </b-col>
      </b-row>


    </b-container>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          name: '',
          phone: '',
          email: '',
          message: ''
        }
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        alert(JSON.stringify(this.form))
      }
    }
  }
</script>
