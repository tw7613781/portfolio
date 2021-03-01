<template>
  <div id="app">
    <div id="nav">
      <ul>
        <li>
          <img src="./assets/logo.png" alt="" />
        </li>
        <li>
          <router-link to="/">Home</router-link>
        </li>
        <li>
          <router-link to="/about">About</router-link>
        </li>
      </ul>
    </div>
    <router-view />
    <div id="footer"></div>
  </div>
</template>

<style lang="scss">
@import "./scss/_base.scss";
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  font-size: $font-size;
  color: $gray;
  background-color: $background;
}

#nav {
  width: 100vw;
  background-color: $primary;
  margin: 0;

  ul {
    list-style: none;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    margin: 0;
    height: 3em;
    padding: 0;

    li {
      padding-right: 2em;
      font-weight: bold;

      a {
        text-decoration: none;
        color: $white;
      }
    }

    img {
      height: 1.5em;
    }
  }

  li:first-child {
    margin-right: auto;
    margin-left: 2em;
  }
}
</style>
