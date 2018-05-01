<template>
  <div id="app">
    <nav>
        <ul class="nav__left">
          <li>
            <router-link to='/'>Home</router-link>
          </li>
          <li>
            <router-link to='/admin'>Admin</router-link>
          </li>
          <li>
            <router-link to='/cart'>Cart</router-link>
          </li>
        </ul>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style lang='scss'>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  background-color: #2c3e50;
  height: 3rem;
  display: flex;
  align-items: center;
}

.nav__left {
  list-style: none;
  display: flex;
  width: 100%;

  & li {
    flex: 0 0 10%;
    & > * {
      text-decoration: none;
      color: white;
    }
  }
}
</style>
