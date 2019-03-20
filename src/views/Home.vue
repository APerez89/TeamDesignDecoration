<template>
  <div class="home">
    <HomeContent msg="Team Design & Decoration"/>
    <Projects/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeContent from '@/components/HomeContent.vue';
import Projects from '@/components/Projects.vue';

export default {
  name: 'home',
  components: {
    HomeContent,
    Projects,
  },
};
</script>

<style lang="scss" scoped>
// HOME STYLES
.home {
  padding: 15px;
}
</style>
