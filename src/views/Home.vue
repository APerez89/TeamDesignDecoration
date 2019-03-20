<template>
  <div class="home">
    <HomeContent msg="Team Design & Decoration"/>
    <div class="cover-img"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeContent from '@/components/HomeContent.vue';

export default {
  name: 'home',
  components: {
    HomeContent,
  },
};
</script>

<style lang="scss" scoped>
// HOME STYLES
.home {
  padding: 15px;
}
</style>
