<template>
  <nav class="nav">
    <router-link class="nav-link active" aria-current="page" to="/"
      >Home</router-link
    >
    <router-link class="nav-link" to="/about">About</router-link>
    <router-view></router-view>
  </nav>
</template>
