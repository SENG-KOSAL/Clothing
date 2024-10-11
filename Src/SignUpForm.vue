<template>
  <div class="signup-wrapper">
    <div class="signup-container">
      <!-- Tabs for Sign up / Log in -->
      <div class="tab-container">
        <button class="tab active">Sign up</button>
        <button class="tab">Log in</button>
      </div>

      <!-- Sign up Form Content -->
      <h2>Sign up</h2>

      <!-- Social Sign up buttons -->
      <div class="social-buttons">
        <button class="social-button fb-button">
          <i class="fab fa-facebook"></i> Sign up with Facebook
        </button>
        <button class="social-button google-button">
          <i class="fab fa-google"></i> Sign up with Google
        </button>
      </div>

      <!-- Divider -->
      <div class="divider">
        <hr /> <span>OR</span> <hr />
      </div>

      <!-- Form Inputs -->
      <form @submit.prevent="handleSubmit">
        <div class="input-row">
          <input type="text" placeholder="First name" v-model="firstName" />
          <input type="text" placeholder="Last name" v-model="lastName" />
        </div>
        <input type="email" placeholder="Email address" v-model="email" />

        <button type="submit" class="signup-button">Sign up</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: '',
      lastName: '',
      email: '',
    };
  },
  methods: {
    handleSubmit() {
      console.log('Form submitted:', this.firstName, this.lastName, this.email);
      // Implement form submission logic here
    },
  },
};
</script>

<style scoped>
/* Wrapper to center the form */
.signup-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(120deg, rgba(255, 153, 240, 0.3), rgba(204, 204, 255, 0.3));
}

/* Container for the signup form */
.signup-container {
  background: white;
  border-radius: 15px;
  padding: 20px;
  width: 400px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  text-align: center;
}

/* Tab buttons */
.tab-container {
  display: flex;
  justify-content: center;
  margin-bottom: 20px;
}
.tab {
  width: 50%;
  padding: 10px;
  border: none;
  background: none;
  cursor: pointer;
}
.tab.active {
  font-weight: bold;
  border-bottom: 3px solid black;
}

/* Title */
h2 {
  margin: 20px 0;
  font-size: 24px;
}

/* Social buttons */
.social-buttons {
  margin-bottom: 20px;
}
.social-button {
  width: 100%;
  padding: 10px;
  border: 1px solid lightgray;
  border-radius: 5px;
  margin-bottom: 10px;
  font-size: 16px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}
.fb-button {
  background-color: #3b5998;
  color: white;
}
.google-button {
  background-color: white;
  color: black;
  border: 1px solid gray;
}

/* Divider */
.divider {
  display: flex;
  align-items: center;
  margin: 20px 0;
}
.divider hr {
  flex: 1;
  border: none;
  border-top: 1px solid lightgray;
}
.divider span {
  padding: 0 10px;
  font-size: 12px;
  color: gray;
}

/* Form */
form {
  display: flex;
  flex-direction: column;
}
.input-row {
  display: flex;
  gap: 10px;
}
input {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid lightgray;
  border-radius: 5px;
}

/* Sign up button */
.signup-button {
  padding: 10px;
  background-color: lightgray;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}
.signup-button:hover {
  background-color: gray;
}
</style>
