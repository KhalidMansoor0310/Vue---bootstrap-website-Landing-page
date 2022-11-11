<template>
  <div>
    <ul class="nav">
      <div class="container">
        <div class="col-10 m-auto">
          <div class="row">
            <div class="col-md-6 d-flex justify-content-center">
              <li class="nav-item logo">
                <router-link
                  class="nav-link text-dark d-flex justify-content-left align-items-center"
                  aria-current="page"
                  to="/"
                >
                  <h1>tado°</h1>
                  <span class="logo__powered-text p-2">powered by</span>
                  <img
                    src="./assets/icons/logo.png"
                    class="logo__image"
                    alt=""
                  />
                </router-link>
              </li>
            </div>
            <div class="col-md-6 d-flex justify-content-center">
              <li class="nav-item navbar__right-col">
                <router-link class="nav-link" to="/about">
                  <img src="./assets/icons/Laag 10.png" alt="" /><br />
                  <span class="text-dark">Beoordeling 4.9 / 5.0</span>
                </router-link>
              </li>
            </div>
          </div>
        </div>
      </div>
    </ul>

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

.logo__powered-text {
  font-size: 12px;
}
@media screen and (max-width: 512px) {
  .logo__powered-text {
    font-size: 10px;
  }
  .navbar__right-col {
    margin-top: -5%;
  }
  .logo__image {
    width: 100px;
  }
  .navbar__right-col {
    margin-left: 0px;
  }
}
.logo {
  margin-left: 30px;
}
</style>
