<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <router-link class="navbar-brand" to="/">
      <img src="favicon.svg" alt="DLMJ"/>
    </router-link>
    <button class="navbar-toggler" type="button"
            data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false"
            aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav navbar-right mr-auto">
        <li class="nav-item" v-bind:class="{ bold:$route.name==='Home' }">
          <router-link class="nav-link" to="/">
            <span class="sr-only" >Home</span>
          </router-link>
        </li>
        <li class="nav-item" v-bind:class="{ bold:$route.name==='About' }">
          <router-link class="nav-link" to="about">
            <span class="sr-only" >About</span>
          </router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style>
#vue-navbar {
  height: 4rem;
  padding-left: 2rem;
  padding-right: 2rem;
  padding-top: 0.3125rem;
  padding-bottom: 0.3125rem;
  position: fixed;
  top: 0;
  z-index: 1;
  width: 100%;

}
.bold {
  font-weight: bolder;
  background: darkgray;
  background-blend-mode: darken;
  height: 100%;
  border-radius: 3px;
}

.navbar-brand {
  height: 100%;
  padding-top: 0rem;
  padding-bottom: 0rem;
}
.navbar-brand > img {
  height: 100%;
}
</style>
