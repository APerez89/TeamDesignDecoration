<template>
  <div id="app">
    <div id="nav-wrap">
      <a href="/home" class="logo"> <img src="/img/logo.png" alt="TDD Logo"> </a>
      <div class="nav">
        <a href="#" class="link">About</a>
        <a href="#" class="link">Projects</a>
        <a href="#" class="link">Contact</a>
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
  --bkgr-light-gray: #f6f6f6;
  --header-lg-mb: 28px;
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
        padding-left: 16px;
        &:visited {
          color: var(--dark-gray);
        }
      }
    }
  }
}

h1 {
  font-size: var(--header-lg-mb);
  font-weight: 100;
  color: var(--dark-gray);
  padding-bottom: 20px;
}
</style>
