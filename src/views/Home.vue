<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <img src="img/cover-img.jpg" alt="">
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'home',
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss" scoped>
// HOME STYLES
.home {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  img {
    max-width: 950px;
    height: 650px;
    padding: 30px;
  }
}
</style>
