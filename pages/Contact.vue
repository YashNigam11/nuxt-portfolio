<template>
  <div class="contact-form" id="contact">
    <h2>Contact Us</h2>
    <form @submit.prevent="submitForm">
      <label for="name">Name</label>
      <input type="text" id="name" v-model="name" required />
      <label for="email">Email</label>
      <input type="email" id="email" v-model="email" required />
      <label for="message">Message</label>
      <textarea id="message" v-model="message" required></textarea>
      <button type="submit" class="btn-submit">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    submitForm() {
      console.log("Name:", this.name);
      console.log("Email:", this.email);
      console.log("Message:", this.message);
      this.name = "";
      this.email = "";
      this.message = "";
    },
  },
};
</script>

<style scoped>
.contact-form {
  display: flex;
  flex-direction: column;
  /* height: 100vh; */
  padding: 25px;
  text-align: center;
}
form {
  text-align: left;
}
h2 {
  font-size: 2.25rem;
  /* font-style: oblique; */
}

label {
  display: block;
  font-size: 1.2rem;
  margin-top: 20px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  font-size: 1rem;
  border-radius: 4px;
  border: 1px solid #ccc;
  margin-top: 5px;
  color: white;
}

button.btn-submit {
  background-color: saddlebrown;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  font-size: 1rem;
  margin-top: 20px;
  cursor: pointer;
}
</style>
