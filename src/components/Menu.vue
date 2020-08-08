<template>
  <div class="menu">
    <div class="logo">
      Subscribr.
    </div>
    <div class="menu_list">
      <router-link class="menu_item" active-class="menu_active" to="/about">
      <p class="rel cv">About Subscribr</p>
    </router-link>
      <router-link class="menu_item" active-class="menu_active" to="/whitepaper">
      <p class="rel whitepaper">Whitepaper</p>
    </router-link>
    <router-link class="menu_item" active-class="menu_active" to="/sdk">
      <p class="rel sdk">SDK</p>
    </router-link>
    <router-link class="menu_item" active-class="menu_active" to="/community">
      <p class="rel community">Community</p>
    </router-link>
    </div>
  </div>
</template>

<style lang="scss">
.logo {
  text-align: center;
  font-size: 24px;
  padding: 30px 0 60px 0;
}
.menu_item {
  text-decoration: none;
}
.menu_item p {
  color: #7c899c;
  padding: 15px 0 15px 30px;
}
.menu_item p::before {
  margin-right: 20px;
  content: '';
}
.menu_active p {
  color: #070e17;
  font-weight: bold;
  background-color: #ced2d9;
}
</style>