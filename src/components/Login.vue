<template>
  <div>
    <h3>Auth Login</h3>
    <p v-if="$route.query.redirect">
      You need to login first.
    </p>
    <form @submit.prevent="login">
      <p v-if="error" class="error">Bad login information</p>
      <div style="margin-bottom: 10px;">
        <input v-model="user" placeholder="username/email">
      </div>
      <div style="margin-bottom: 10px;">
        <input v-model="password" placeholder="password" type="password">
      </div>
      <button type="submit">login</button><br>
    </form>
  </div>
</template>

<script>
export default {
  data () {
    return {
      user: '',
      password: '',
      error: false
    }
  },
  methods: {
    login () {
      alert('login ok.')
    }
  }
}
</script>

<style>
.error {
  color: red;
}
</style>
