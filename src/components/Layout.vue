<template>
  <div>
    <b-navbar fixed="top" style="opacity: 0.9" class="navbar" type="dark" variant="dark">
      <b-navbar-brand href="#">
        <img src="../assets/logo.png" height="30" class="d-inline-block align-top">
      </b-navbar-brand>
      <b-navbar-nav>
        <b-nav-item to="/" href="#">Home</b-nav-item>
        <b-nav-item to="/series" href="#">Series</b-nav-item>
        <b-nav-item to="movies" href="#">Movies</b-nav-item>
      </b-navbar-nav>
       <b-navbar-nav class="ml-auto">
        <p class="flex mr-2 mt-2" style="color: grey">Account</p>
       <b-avatar class="right: 0;" button @click="onClick" src="https://lh3.googleusercontent.com/ogw/ADea4I64PuJ21nHejw7x6_4OWa28pNTGyhWjU4_ewGUWeGQ=s32-c-mo"></b-avatar>
       </b-navbar-nav>
    </b-navbar>

    <router-view/>
  </div>
</template>

<style>
</style>
