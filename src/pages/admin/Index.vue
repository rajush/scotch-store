<template>
<div>
  <div class="admin-new">
    <div class="container">
      <div class="col-lg-3 col-md-3 col-sm-12 col-xs-12">
        <ul class="admin-menu">
          <!-- Links are to sibling routes -->
          <li>
            <router-link to="/admin">View Products</router-link>
          </li>
          <li>
            <router-link to="/admin/new">New Product</router-link>
          </li>
        </ul>
      </div>
      <!-- Outlet for children routes -->
      <router-view></router-view>
    </div>
  </div>
</div>
</template>

<script>
export default {};
</script>

<style lang="css">
.admin-new,
.admin-products,
.product-details {
  border-bottom: 2px solid #f5f5f5;
  padding: 30px 0;
}

.admin-menu a {
    display: block;
    background: #efdb06;
    border: 1px solid #f9e610;
    color: #3d3d3d;
    padding: 10px 15px;
    font-family: PT Sans,sans-serif;
    font-weight: 700;
    text-transform: uppercase;
    font-size: 12px;
    -webkit-transform: scaleX(1);
    transform: scaleX(1);
    -webkit-transition: -webkit-transform .2s ease-in;
    transition: -webkit-transform .2s ease-in;
    transition: transform .2s ease-in;
    transition: transform .2s ease-in,-webkit-transform .2s ease-in;
}

.admin-menu a:hover {
    text-decoration: none;
    -webkit-transform: scaleX(1.02);
    transform: scaleX(1.02);
}

.admin-menu>li {
  text-align: left;
}
</style>
