<template>
  <div id="app">
    <header>
      <h1>Welcome to NCI Page</h1>
      <img src="https://via.placeholder.com/60" alt="Organization Image">

    </header>
    <form>
      <div class="form-group">
        <label for="username">Username</label>
        <input type="text" id="username" v-model="username" placeholder="Enter your username">
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" v-model="password" placeholder="Enter your password">
      </div>
      <button @click.prevent="login">Login</button>
    </form>
    <section>
      <p>Developed by Applift Technologies</p>
    </section>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    login() {
      // Implement your login logic here
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  overflow: hidden;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  font-weight: bold;
}

input {
  width: 80%;
  padding: 10px;
  font-size: 16px;
  border-radius: 5px;
  border: 1px solid #ccc;
}
form {
width: 100%;
}
button {
  padding: 10px 20px;
  font-size: 16px;
  background-color: #2c3e50;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

p {
  margin-top: 20px;
}
</style>