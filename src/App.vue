<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <ul>
      <li><router-link to="/">首 页</router-link></li>
      <li><router-link to="/login">登 录</router-link></li>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome Fwlink App'
    }
  },
  methods: {
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-color: #f3f3f3;
}
#app {
  max-width: 800px;
  min-height: 800px;
  margin-left: auto;
  margin-right: auto;
  padding: 18px;
  background-color: #fff;
}
h1 {
  margin-top: 0;
  padding-left: 10px;
  border-radius: 5px;
  background-color: #e3e3e3;
}
a {
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
</style>
