<template>
  <div id="app">
    <div class="wrapper">
      <div class="side_content">
        <Menu />
      </div>
      <div class="main_content">
        <div class="main_top">
          <TopLine />
        </div>
        <div class="main_middle">
          <router-view/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Menu from '@/components/Menu.vue';
import TopLine from '@/components/TopLine.vue';

export default {
  components: {
    Menu, TopLine
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}
@font-face {
  font-family: regular;
  src: url(assets/fonts/GillSans-Bold.otf);
}
@font-face {
  font-family: roboto;
  src: url(assets/fonts/Roboto.ttf);
}
html {
  font-family: roboto;
}
.wrapper { 
  width: 90%;
  height: 100%;
  min-height: 950px;
  display: flex;
}
.side_content{
  width: 360px;
  height: 100%;
  min-height: 950px;
  background-color: #fff;
}
.main_content {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
  min-height: 950px;
  background-color: #F5F7FA;
}
.main_top {
  width: 100%;
  height: 70px;
  padding: 0 50px;
}
.main_middle {
  padding: 0 50px;
}




#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
