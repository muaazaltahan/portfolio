<template>
  <div class="projects">
    <AllProjects
      v-for="project in projects"
      :key="project.id"
      :title="project.title"
      :image="require(`@/assets/${project.image}`)"
      :desc="project.desc"
      :gpurl="project.gpurl"
      :curl="project.curl"
    />
  </div>
</template>

<script>
import AllProjects from "@/components/AllProjects.vue";
import JsonProjects from "@/projects.json";
export default {
  name: "Projects",
  components: {
    AllProjects,
  },
  data: function () {
    return {
      projects: JsonProjects,
    };
  },
};
</script>
