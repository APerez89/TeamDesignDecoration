<template>
  <div class="home">
    <HomeContent msg="Team Design & Decoration"/>
    <About/>
    <Projects/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeContent from '@/components/HomeContent.vue';
import About from '@/components/About.vue';
import Projects from '@/components/Projects.vue';

export default {
  name: 'home',
  components: {
    HomeContent,
    About,
    Projects,
  },
};
</script>

<style lang="scss" scoped>
// HOME STYLES
.home {
  padding: 0px 15px;
  text-align: center;
}
</style>
