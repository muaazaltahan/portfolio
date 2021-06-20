<template>
  <div class="nav">
    <router-link to="/">
      <div class="nav-item">
        <img src="../assets/hm.png" alt="Home">
      </div>
    </router-link>
    <router-link to="/about">
      <div class="nav-item">
        <img src="../assets/ab.png" alt="About">
      </div>
    </router-link>
    <router-link to="/projects">
      <div class="nav-item">
        <img src="../assets/cg2.png" alt="About">
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: "Nav",
};
</script>

<style scoped lang="scss">
.nav {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  background: #55fa;
  display: flex;
  justify-content: center;
  a {
    font-weight: bold;
    color: #ff5;
    &.router-link-exact-active .nav-item {
      background: #55fc;
    }
    .nav-item {
      width: 50px;
      text-align: center;
      float: right;
      transition: background 0.2s;
      padding: 5px;
      img{
        width: 35px;
        height: 35px;
      }
    }
    .nav-item:hover {
      background: #55fc;
    }
  }
}
</style>