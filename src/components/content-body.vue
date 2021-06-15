<template>
  <div id="vue-content-body">
    <modal v-show="isModalVisible" @close="closeModal">
      <template v-slot:header>
        <h1>Terms and Conditions</h1>
      </template>
      <template v-slot:body>
        <h1>blah blah</h1>
      </template>
      <template v-slot:footer>
        <input id="modal-eula-submit" type="submit" class="btn btn-primary" value="Pray">
      </template>
    </modal>
    <section id="cloud-banner">
      <article>
        <div class="eula container">
          <div class="row" style="padding-top: 40%;">
            <div class="col-3"></div>
            <div class="col-6">
              <label for="eula-submit" class="form-check-label">
                Would you accept Jesus Christ as your lord and savior?
              </label>
            </div>
            <div class="row">
              <button type="button" class="btn" @click="showModal"><input id="eula-submit" type="submit" class="btn btn-primary" value="Yes"></button>
            </div>
          </div>
        </div>
      </article>
    </section>
  </div>
</template>

<script>
import modal from './modal'

export default {
  name: 'content-body',
  components: {
    modal
  },
  data() {
    return {
      isModalVisible: false,
    };
  },
  methods: {
    showModal() {
      this.isModalVisible = true;
    },
    closeModal() {
      this.isModalVisible = false;
    }
  }
};

</script>


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
  background-image: url("~@/assets/scroll.png");
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