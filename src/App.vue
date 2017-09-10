<template>
<div id="app">
  <!-- <img src="./assets/logo.png"> -->
  <nav>
    <div class="container">
      <ul class="nav__left">
        <!-- Navigation Links -->
        <li>
          <router-link to="/">Home</router-link>
        </li>
        <li>
          <router-link to="/admin">Admin</router-link>
        </li>
        <li>
          <router-link to="/cart">Cart</router-link>
        </li>
      </ul>
    </div>
  </nav>

  <!-- Route Outlet -->
  <router-view></router-view>
</div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

nav {
  font-family: 'PT Sans', sans-serif;
  font-weight: 700;
  border-bottom: 2px solid #F5F5F5;
  text-transform: uppercase;
}

nav .container {
  display: flex;
}

nav .nav__left {
  flex-grow: 3;
  display: flex;
}

nav .nav__right {
  flex-grow: 2;
  display: flex;
  flex-direction: row-reverse;
}

nav li a {
  color: #3D3D3D;
  background: #FFF;
  display: block;
  padding: 15px 15px;
  transition: all 150ms ease-out;
}

nav li a:hover {
  text-decoration: none;
  color: #FFF;
  background: #EFDB06;
}

nav li a:focus {
  text-decoration: none;
  color: #3D3D3D;
}
</style>
