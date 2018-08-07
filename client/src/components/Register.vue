<template>
  <div id="register">
    <h1> Register </h1>
    <input
      type="email"
      name="email"
      v-model="email"
      placeholder="Email"
    >>
    <br>
    <input
      type="password"
      name="password"
      v-model="password"
      placeholder="Password"
    >>
    <br>
    <button>Register</button>>
  </div>
</template>

<script>
export default {
  data () {
    return {
      email: 'abc',
      password: '123'
    }
  },
  watch: {
    email (value) {
      console.log('Email has changed', value)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
