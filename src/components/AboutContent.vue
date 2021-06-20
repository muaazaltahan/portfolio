<template>
  <div class="about">
    You can contact me at: <br>
    <a target="_blank" href="https://www.facebook.com/DeveloperMuaaz/">
      <img src="../assets/fb.png">Facebook
    </a>
    <a target="_blank" href="https://t.me/muaazaltahan">
      <img src="../assets/tel.png">Telegram
    </a>
    <a target="_blank" href="mailto:almuuaz559@gmail.com">
      <img src="../assets/el.png">E-mail
    </a>
    <br>
    <img src="../assets/phn.png">Phone Number: +963 967 497 434
    <div class="thanks">
      Thanks For Visiting My Website. <br>
      See My Other Projects <router-link to="/projects">Here</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutContent",
};
</script>

<style scoped lang="scss">
img {
  width: 40px;
  height: 40px;
  transition: width 0.2s, height 0.2s;
}
img:hover {
  width: 43px;
  height: 43px;
}
.about {
  background: #0005;
  padding: 20px;
  margin: 20px;
  text-align: center;
  a {
    color: #ff5;
    display: inline-block;
    padding: 10px;
  }
  .thanks{
    margin: 20px;
    font-size: 20px;
  }
}
</style>