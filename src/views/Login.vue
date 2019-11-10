<template>
  <div class="container">
    <h1 class="text-center">User Login</h1>
      <div class="container pt-3">
        <div class="row justify-content-sm-center">
          <div class="col-sm-6 col-md-4">

            <div class="card border-info text-center">
              <div class="card-header">
                Sign in to continue
              </div>
              <div class="card-body">
                <img src="https://i1248.photobucket.com/albums/hh483/hilarion18/RPV%20WS.png" border="0" alt=" photo RPV.png" height=100 width=100>
                <h4 class="text-center">Papua untuk bangsa</h4>
                <form class="form-signin">
                  <input type="text" class="form-control mb-2" placeholder="Email or phone number" required autofocus>
                  <input type="password" class="form-control mb-2" placeholder="Password" required>
                  <button class="btn btn-lg btn-primary btn-block mb-1" type="submit">Login</button>
                  <label class="checkbox float-left">
                    <input type="checkbox" value="remember-me">
                    Remember me
                  </label>
                  <a href="#" class="float-right">Lupa password?</a>
                </form>
              </div>
            </div>
            <a href="#" class="float-right">Create an account </a>
          </div>
        </div>
      </div>
  </div>
</template>

<style>
  .card {
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
</style>
