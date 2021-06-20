<template>
  <div class="who-am-i">
    <img src="../assets/logo.png" alt="MUAAZ AL-TAHAN">
    <h1>Here Is My Vue.js Project</h1>
    <div class="my-desc">
      I am a front end developer. <br>
      These are my skills:
      <ul>
        <li>HTML5</li>
        <li>CSS3</li>
        <li>JS</li>
        <li>AJAX, JSON, JQuery, Bootstrap</li>
        <li>Vue.js</li>
      </ul>
    </div>
    <div class="my-desc">
      I have been working with html,css,js for two years but this year I learned Vue.js to improve my self.<br>
      I created some projects with bootstrap & jquery but i don't realy like them because i don't like using fixed content i love to build everything by my self.
    </div>
  </div>
</template>

<script>
export default {
  name: 'WhoAmI'
}
</script>

<style scoped lang="scss">
.who-am-i{
  text-align: center;
  img{
    width: 200px;
  }
  h1{
    font-size: 20px;
  }
  .my-desc{
    background: #0005;
    text-align: left;
    font-size: 18px;
    padding: 5px;
    margin: 10px 0;
    line-height: 1.5;
    ul{
      padding: 15px;
    }
  }
}
</style>
