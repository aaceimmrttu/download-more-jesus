<template>
  <content id="vue-content-body">
    <section id="cloud-banner">
      <article></article>
    </section>
      <header> Have you accepted Jesus Christ as your lord and savior? 基督</header> 
      <div class="eula container">
        <div class="row">
          <div class="col-4">
            <textarea id="eula-terms" class="w-100">eula</textarea>
          </div>
        </div>
        <div class="row">
          <div class="col-3">
            <label for="eula-accept" class="form-check-label">I accept Jesus Christ as my lord and savior</label>
          </div>
          <div class="col-1">
            <input id="eula-accept" type="checkbox" class="form-check-input">
          </div>
        </div>
        <div class="row">
          <div class="col-2">
            <input id="eula-submit" type="submit" class="btn btn-primary" value="Amen">
            </div>
        </div>
      </div>
  </content>
</template>


<style>
header {
  color: red;
}
#vue-content-body {

  height: 100%;
  width: 100%;
  resize: both;
  padding-top: 4rem;
}
#cloud-banner {
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0.5), rgba(0, 0, 255, 0.521)),
  url("~@/assets/background.webp");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100%;
  width: 100%;
  height: 600pt;
  padding-top: 30px;
  padding-bottom: 30px;

}
#cloud-banner > article {
  background-image: url("https://png2.cleanpng.com/sh/eb3254700755777743847c5d78e9bef0/L0KzQYi4UsA5N5U5S5GAYULkQ4jsUBFiOJc1TZC6MUa6QIa9VcE2OWM8Sag7NUm5SYe9TwBvbz==/5a2a37e3aa0f05.1167056515127162596966.png");
  background-size: 700px 700px;
  margin-left: auto;
  margin-right: auto;
  width: 700px;
  height: 700px;
  margin-top: 40px;
}
.form-inline > input {
  display: inline;
  width: 150pt;
}
</style>