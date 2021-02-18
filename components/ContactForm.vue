<template>
  <div>
    <div class="p-2 pb-3 text-center contact-title">
      <h1>
        Contact Us
      </h1>
    </div>

    <div class="form">
      <b-container>
        <b-form class="form-container">
          <b-form-group
            id="input-group-1"
            label="Name"
            label-for="input-1"
          >
            <b-form-input
              id="input-1"
              v-model="form.name"
              type="text"
              required
              placeholder="Frodo Baggins"
            />
          </b-form-group>

          <b-form-group
            id="input-group-2"
            label="email"
            label-for="input-2"
            description="Your email is never shared!"
          >
            <b-form-input
              id="input-2"
              v-model="form.email"
              type="email"
              required
              placeholder="frodo@theshire.com"
            />
          </b-form-group>

          <b-form-group
            id="input-group-3"
            label="Message"
            label-for="input-3"
          >
            <b-form-textarea
              id="input-3"
              v-model="form.message"
              type="textarea"
              placeholder="Say hello..."
              rows="3"
              max-row="6"
            />
          </b-form-group>
          <b-button type="submit" class="button">
            Send
          </b-button>
        </b-form>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      form: {
        name: '',
        email: '',
        message: ''
      }
    }
  },
  methods: {
    onSubmit () {},
    onReset () {}
  }
}
</script>

<style>
  .form {
    background: rgb(131,126,222);
background: radial-gradient(circle, rgba(131,126,222,1) 5%, rgba(81,12,96,1) 58%, rgba(0,0,0,1) 100%);
  }
  .form-container {
    width: 500px;
  }

  .contact-title {
    background-color: black;
    color: rgb(158, 26, 158);
    margin: -10px;
  }

  .button {
    background-color: purple;
  }

  .button:hover {
    background-color: black;
    transform: scale(1.2, 1.2);
  }
</style>
