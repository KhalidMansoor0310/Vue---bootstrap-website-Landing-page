<template>
  <div class="container my-5 laag">
    <div class="row d-flex justify-content-center align-items-center">
      <div class="col-12 col-lg-6 col-md-6 col-sm-12">
        <img :src="laag12" class="img__laag" alt="" />
      </div>
      <div class="col-12 col-lg-4 col-md-4 col-sm-12">
        <h5 class="laag__text-heading my-3">
          Er werken al 2 miljoen mensen met Tado!
        </h5>
        <p class="laag__text-paragraph">
          <span class="">
            leert je leefritme kennen en past de verwarming daarop aan.</span
          >
          tado° laat het je weten als alle bewoners het huis verlaten hebben of
          als er een raam openstaat. Je kunt thuis én op afstand je verwarming
          bedienen. tado° kan meerdere kamers of zones apart verwarmen met een
          extra thermostaat of
        </p>
      </div>
    </div>
  </div>
</template>
<script>
import laag12 from "../assets/img/Laag 12.png";
export default {
  data() {
    return {
      laag12: laag12,
    };
  },
};
</script>

<style scoped>
@font-face {
  font-family: Freizeit-extraBold;
  src: url("../assets/fonts/Freizeit/Freizeit-ExtraBold.otf");
}
.laag__text-heading {
  color: #00b969;
  font-family: Freizeit-extraBold;
}
.img__laag {
  width: 100%;
}
.laag {
  /* font-family: "Freizeit"; */
}

.laag__text-paragraph {
  font-size: 18px;
}
.laag__text-paragraph span {
  font-family: Freizeit-extraBold;
}
</style>
