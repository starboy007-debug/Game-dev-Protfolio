<template>
  <div>
    <h1>Games</h1>

    <div style="margin-bottom: 30px;">
      Here are some games I've created, either to be released, or during game jams, or to showcase my skills using Unity.
    </div>

    <ProjectsList v-bind:projects="projects" />

    <div style="margin-top: 20px;">
      More on <a target="_blank" href="https://starboy007-debug.itch.io/">pavan.itch.io</a>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import ProjectsList from "@/components/ProjectsList.vue";
import gameProjectsData from "@/data/GameProjectsData.ts";

export default Vue.extend({
  name: "GameProjects",
  components: {
    ProjectsList,
  },
  data: function () {
    return {
      projects: gameProjectsData,
    };
  },
});
</script>
