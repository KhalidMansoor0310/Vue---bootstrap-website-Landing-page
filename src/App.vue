<template>
  <div>
    <b-navbar toggleable="lg" class="px-5" type="dark" variant="light">
      <b-navbar-brand
        ><router-link
          class="navbar-brand text-dark d-flex justify-content-center align-items-center"
          aria-current="page"
          to="/"
        >
          <h1>tado°</h1>
          <span class="logo__powered-text p-2">powered by</span>
          <h2 class="fw-bold">Nerds</h2>
        </router-link></b-navbar-brand
      >

      <b-navbar-toggle target="nav-collapse" class="bg-dark"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ms-auto">
          <router-link class="nav-link" to="/about">
            <img src="./assets/icons/Laag 10.png" alt="" /><br />
            <span class="text-dark">Beoordeling 4.9 / 5.0</span>
          </router-link>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-family: "Ferzeit";
}

.nav {
  padding: 30px;
  font-family: "Ferzeit";

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      // color: #42b983;
      font-size: 30px;
      color: #000000;
      font-family: "Freizeit";
    }
  }
  .logo__powered-text {
    font-size: 12px;
  }
  b-navbar {
    font-family: "Ferzeit";
  }
}
</style>
