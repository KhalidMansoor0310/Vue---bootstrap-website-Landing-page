<template>
  <div class="footer mt-5">
    <div class="container">
      <div class="col-10 col-lg-10 col-md-10 col-sm-12 py-5 m-auto">
        <div class="row m-auto">
          <div class="col-12 m-auto col-lg-6 col-md-5 col-sm-12">
            <h2>
              Start ook met besparen en kies voor een tado° slimme thermostaat
            </h2>
            <!-- <div class="col-12 col-lg-8 col-md-8 col-sm-12"> -->
            <button class="btn text-white">
              Ja, ik wil meer informatie kopiëren<i
                class="fa-solid fa-arrow-right p-2"
              ></i>
            </button>
            <!-- </div> -->
          </div>
          <div
            class="col-12 col-lg-6 col-md-6 col-sm-12 d-flex justify-content-center align-items-center"
          >
            <img :src="laag11" class="footer__laag-img" alt="" />
          </div>
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
  font-family: Freizeit-bold;
}
@font-face {
  font-family: Freizeit-bold;
  src: url("../assets/fonts/Freizeit/Freizeit-Bold.otf");
}
h2 {
  font-size: 40px;
  color: #fffefe;
  /* font-weight: bold; */
  font-family: Freizeit-bold;
}
button {
  border-radius: 27px;
  background-color: #00b969;
}
@media screen and (max-width: 576px) {
  button {
    font-size: 12px;
  }
}

.footer__laag-img {
  width: 100%;
}
</style>
