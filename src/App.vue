<template>
  <div id="app">
    <div id="nav-wrap">
      <div class="nav">
        <router-link class="link" to="/">Home</router-link>
        <router-link class="link" to="/about">About</router-link>
        <router-link class="link" to="/projects">Projects</router-link>
      </div> <!-- Nav End -->
    </div> <!-- Nav Wrap End -->
    <router-view/>
  </div> <!-- App End -->
</template>

<style lang="scss">
// GLOBAL STYLES
* {
  box-sizing: border-box;
  margin: 0px;
  border: 1px solid red;
}

#app {
  #nav-wrap {
    width: 100%;
    height: 250px;
    background-color: blue;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    .nav {
      margin-bottom: 30px;
      .link {
        padding: 0px 20px;
        text-decoration: none;
        font-size: 21px;
        &:visited {
          color: #fff;
        }
        &:hover {
          color: red;
        }
      }
    }
  }
}
</style>
