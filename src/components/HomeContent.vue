<template>
  <div class="home-content">
    <h1>{{ msg }}</h1>
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
}
</style>
