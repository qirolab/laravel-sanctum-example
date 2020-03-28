<template>
  <nav class="navbar navbar-expand navbar-dark bg-dark">
    <div class="container">
      <div class="navbar-header">
        <router-link class="navbar-brand" to="/">Laravel Sanctum</router-link>
      </div>
      <ul class="nav navbar-nav">
        <router-link class="nav-item nav-link" :to="{ name: 'Login' }">
          Login
        </router-link>
        <router-link class="nav-item nav-link" :to="{ name: 'Register' }">
          Register
        </router-link>
        <router-link class="nav-item nav-link" :to="{ name: 'Dashboard' }">
          Dashbord
        </router-link>
        <a class="nav-item nav-link" href="#">Logout</a>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style>
.router-link-exact-active {
  color: #ffffff !important;
  transition: all 0.25s;
}
</style>
