<template>
  <div class="footer mt-5">
    <div class="container my-5">
      <div class="row py-5">
        <div
          class="col-12 col-lg-6 col-md-6 col-sm-12 d-flex justify-content-center align-items-center"
        >
          <div class="row">
            <h2>
              Start ook met besparen en kies voor een tado° slimme thermostaat
            </h2>
            <div class="col-md-8">
              <button class="btn btn-lg btn-block text-white bg-success">
                Ja, ik wil meer informatie kopiëren
              </button>
            </div>
          </div>
        </div>
        <div
          class="col-12 col-lg-6 col-md-6 col-sm-12 d-flex justify-content-center align-items-center"
        >
          <img :src="laag11" class="footer__laag-img" alt="" />
        </div>
      </div>
    </div>
    <div
      class="container-fluid bg-white d-flex align-items-center justify-content-center"
    >
      <span class="p-4 fw-bold"> tado° powered by Nerds</span>
    </div>
  </div>
</template>

<script>
import laag11 from "../assets/img/Laag 11.png";
export default {
  data() {
    return {
      laag11: laag11,
    };
  },
};
</script>

<style scoped>
.footer {
  background-color: #f9a300;
}
h2 {
  font-size: 51px;
  color: #fffefe;
  font-weight: bold;
  font-family: "Freizeit";
}
button {
  border-radius: 27px;
  background-color: #00b969;
}
.footer__laag-img {
  width: 100%;
}
</style>
