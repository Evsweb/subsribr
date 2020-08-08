<template>
  <div class="top_menu">
    <div class="search">
      <input type="text" name="" id="" placeholder="search...">
    </div>
    <div class="github">GitHub</div>
  </div>
</template>

<style lang="scss">
.top_menu {
  margin-top: 25px;
  width: 90%;
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
}
.search input {
  height: 25px;
  width: 180px;
  border-radius: 15px;
}
.search input::placeholder {
  padding-left: 10px;
}
.github {
  cursor: pointer;
  align-self: center;
}
.github::after {
  content: ""
}
</style>