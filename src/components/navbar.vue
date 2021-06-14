<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#"><img src="favicon.svg" alt="DLMJ"/></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav navbar-right mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
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

.navbar-brand {
  height: 100%;
  padding-top: 0rem;
  padding-bottom: 0rem;
}
.navbar-brand > img {
  height: 100%;
}
</style>
