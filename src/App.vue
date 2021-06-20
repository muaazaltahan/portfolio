<template>
  <div id="app">
    <Nav/>
    <router-view/>
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue';
export default {
  components: {
    Nav
  }
};
</script>

<style lang="scss">
@font-face{
  font-family: hemi-head;
  src: url('assets/hemi-head-bd-it.ttf');
}
*{
  box-sizing: border-box;
}
body{
  font-family: hemi-head;
  background-image: url('assets/bg.svg');
  padding: 50px 0;
  margin: 0;
  color: #fff;
}
ul{
  list-style: none;
  margin: 0;
}
</style>