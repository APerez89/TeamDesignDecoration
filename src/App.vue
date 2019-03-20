<template>
  <div id="app">
    <div id="nav-wrap">
      <a href="#" class="logo"> <img src="/img/logo.png" alt="TDD Logo"> </a>
      <div class="nav">
        <a href="#" class="link">Home</a>
        <a href="#" class="link">About</a>
        <a href="#" class="link">Projects</a>
      </div> <!-- Nav End -->
    </div> <!-- Nav Wrap End -->
    <router-view/>
  </div> <!-- App End -->
</template>

<style lang="scss">
// GLOBAL STYLES
:root {
  --dark-gray : #242424;
  --light-gray: #575757;
  --header-size-mb: 28px;
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
    padding: 15px;
    .logo {
      img {
        width: 65px;
        height: 65px;
      }
    }
    .nav {
      display: flex;
      align-items: flex-end;
      .link {
        font-size: 14px;
        letter-spacing: 1.4px;
        text-decoration: none;
        padding: 0px 16px 0px;
        &:visited {
          color: var(--dark-gray);
        }
      }
    }
  }
}
</style>
