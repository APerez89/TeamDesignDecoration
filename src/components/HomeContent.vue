<template>
  <div class="home-content">
    <h1>{{ msg }}</h1>
    <div class="cover-img">
      <img src="img/cover-img.jpg" alt="">
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
    font-size: 28px;
    font-weight: 100;
    color: var(--dark-gray);
  }
  .cover-img {
    padding: 20px 0px;
    img {
      width: 100%;
    }
  }
}
</style>
