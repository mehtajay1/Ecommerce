<template>
  <nav class="navbar">
    <img class="logoimg" src="../assets/logo.png" />
    <div class="search-data">
      <input type="text" class="base-text-field search-text" />
      <button class=search-button><i class="fa fa-search"></i>Search</button>
    </div>
    <div class="login-data">
      <div class="cart">
        <div class="cart-count">1</div>
        <i class="fa fa-shopping-cart cart-icon"></i>
      </div>
        <button class="base-button-primary">Login</button>

    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.navbar {
  top: 0;
  position: fixed;
  display: flex;
  justify-content: space-between;
  background-color: var(--navbar-color);
  height: 6vh;
  width: 98%;
  padding: 15px;
  box-shadow: 0 3px 20px 3px #c0c0c0;
}

body {
  padding: 0;
  margin: 0;
}
.cart-icon{
  z-index: 1;
  font-size: 32px;
}

.login-data {
  display:flex;
  flex-grow: 2;
  justify-content: space-evenly;
}
.search-text {
  height: 35px;
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
}
.search-data {
  margin-left: 10px;
  margin-right: 10px;
  display: flex;
  flex-grow: 10;
  background-color: var(--navbar-color);
}

.search-button {
  height: 37px;
  background-color: var(--primary-color);
  color: white;
  border:0;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
.search-img {
  height: 100%;
}
.logoimg {
  width: 15%;
  height: 90%;
  flex-grow: 1;
}

.cart-count{
  text-align: center;
  position: absolute;
  height: 16px;
  width: 16px;
  margin-left: 20px;
  font-family: inherit;
  font-size: 12px;
  background-color: var(--primary-color);
  border-radius: 50%;
}
.cart {
  color: white;
  margin: 0 10px;
}
</style>
