<template>
  <div class="projects-container" id="projects">
    <h1>Our Projects</h1>
    <div class="projects">
      <!-- eslint-disable -->
      <div class="project-img-wrap" v-for="(project, idx) in data" :key="idx"> <!-- Next line is to randomly assign number of images -->
        <div class="project-img" @click="projectClick(project.id)"
          :class="['item', `h${randomNumber(7)} v${randomNumber(7)}`]"
        >
          <img :src="`img/proj-img/plc-hld-img/${project.cover}`">
          <h2>{{ project.title }}</h2> <!-- Also v-text="`${project.title}`" will work -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import * as data from '../data.json';

export default {
  name: 'Projects',
  data() {
    return {
      data: data.default,
      picked: [],
    };
  },
  methods: {
    randomNumber(limit) {
      return Math.floor(Math.random() * limit) + 1;
    },
    projectClick(route) {
      this.$router.push(route);
    },
  },
};
</script>

<style lang="scss" scoped>
.projects-container {
  padding: 40px 15px;
  .projects {
    .project-img-wrap {
      padding-bottom: 25px;
      .project-img {
        text-align: left;
        img {
          width: 100%;
        }
        h2 {
          font-family: 'Times New Roman', Times, serif;
          font-size: 32px;
          font-weight: 100;
          margin-top: 5px;
          color: var(--taupe);
        }
      }
    }
    .project-img-wrap:last-child {
      padding-bottom: 0px;
    }
  }
}
</style>
