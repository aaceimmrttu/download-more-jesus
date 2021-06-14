<template>
  <content id="vue-content-body">
    <section id="cloud-banner">
      <article></article>
    </section>
      <header> Have you accepted Jesus Christ as your lord and savior? 基督</header> 
      <div class="eula container">
        <div class="row">
          <div class="col-4">
            <textarea id="eula-terms" class="w-100">{{ eula }}</textarea>
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
