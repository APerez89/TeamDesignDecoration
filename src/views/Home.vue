<template>
  <div class="home" id="home">
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
  text-align: center;
  margin: 20px 0;
}
</style>
