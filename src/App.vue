<template>
  <div id="app">
    <div id="nav-wrap">
      <a href="#" class="logo"> <img src="/img/logo.png" alt="TDD Logo"> </a>
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
:root {
  --dark-gray : #181818;
}

* {
  box-sizing: border-box;
  margin: 0px;
  // border: 1px solid red;
}

#app {
  width: 100%;
  font-family: Arial, Helvetica, sans-serif;
  #nav-wrap {
    width: 100%;
    display: flex;
    justify-content: space-between;
    .logo {
      padding: 5px;
      img {
        width: 65px;
        height: 65px;
        padding: 5px;
      }
    }
    .nav {
      display: flex;
      align-items: flex-end;
      .link {
        font-size: 14px;
        letter-spacing: 1.4px;
        text-decoration: none;
        padding: 0px 20px 12px 0px;
        &:visited {
          color: var(--dark-gray);
        }
      }
    }
  }
}
</style>
