<template>
  <div>
    <div class="project" :title="title" :image="image" :desc="desc" :gpurl="gpurl" :curl="curl">
      <div class="p-title">{{title}}</div>
      <div class="p-image">
        <img :src="image" :alt="title">
      </div>
      <div class="p-desc">{{desc}}</div>
      <div class="p-urls">
        <a :href="gpurl" target="_blank">Show On Github Pages</a> <br>
        <a :href="curl" target="_blank">Code On Github</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AllProjects',
  props: ["title","image","desc","gpurl","curl"]
}
</script>

<style scoped lang="scss">
.project{
  background: #0005;
  margin: 10px;
  overflow: hidden;
    text-align: center;
  .p-title{
    width: 100%;
    font-size: 22px;
  }
  .p-image{
    width: 100%;
    img{
      width: 100%;
    }
  }
  .p-desc{
    width: 100%;
    padding-top: 10px;
    font-size: 18px;
  }
  .p-urls{
    padding: 10px;
    a{
      color: #ff5;
      font-size: 18px;
      padding: 5px;
    }
  }
}
@media screen and (min-width: 600px) {
  .project .p-image{
    width: 50%;
    float: left;
  }
}
@media screen and (min-width: 1200px) {
  .project{
    width: 48%;
    height: 220px;
    float: left;
    .p-image{
      width: 45%;
      img{
        height: 190px;
      }
    }
  }
}
</style>