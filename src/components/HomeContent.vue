<template>
  <div class="home-content">
    <div class="cover-img">
      <img src="img/cover-img2.jpg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeContent',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.home-content {
  h1 {
    padding-bottom: 20px;
  }
  .cover-img {
    padding-bottom: 40px;
    img {
      width: 100%;
    }
  }
}
</style>
