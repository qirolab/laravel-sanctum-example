<template>
  <div class="home col-5 mx-auto py-5 mt-5">
    <h1 class="text-center">Register</h1>
    <div class="card">
      <div class="card-body">
        <div class="form-group">
          <label for="name">Name:</label>
          <input type="name" class="form-control" id="name" />
        </div>
        <div class="form-group">
          <label for="email">Email address:</label>
          <input type="email" class="form-control" id="email" />
        </div>
        <div class="form-group">
          <label for="password">Password:</label>
          <input type="password" class="form-control" id="password" />
        </div>
        <div class="form-group">
          <label for="password_confirmation">Confirm Password:</label>
          <input
            type="password"
            class="form-control"
            id="password_confirmation"
          />
        </div>
        <button type="submit" class="btn btn-primary btn-block">
          Register
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
