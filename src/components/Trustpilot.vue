<template>
  <div class="container trustpilot my-5">
    <div class="row">
      <img :src="laag6" alt="" />
    </div>

    <div class="row d-flex justify-content-center">
      <img
        src="../assets/icons/Laag 10.png"
        class="trustpilot__img my-3"
        alt=""
      />

      <p class="trustpilot__text">Onze klanten beoordelen ons met 4.9 / 5.0</p>
      <div class="col-12 col-lg-3 col-md-4 m-2 p-5 trustpilot__cards card">
        <img :src="greenStars" alt="" class="trust__star-img mb-3" />
        <p>
          Het werkt heel eenvoudig en fijn dat de installatie zo snel kon. Ik
          kan nu deze winter al gaan besparen op mijn energiekosten.
        </p>
        <span class="">L.J. Wood, Vinkeveen</span>
      </div>
      <div class="col-12 col-lg-3 col-md-4 m-2 p-5 trustpilot__cards card">
        <img :src="stars" alt="" class="mb-3 trust__star-img" />
        <p>
          Uitstekend geholpen door Frank. Alles was binnen 30 minuten gepiept en
          ik kon zoveel vragen stellen als ik wil.
        </p>
        <span class="">L.J. Wood,Vinkeveen</span>
      </div>
      <div class="col-12 col-lg-3 col-md-4 m-2 p-5 trustpilot__cards card">
        <img :src="stars" alt="" class="mb-3 trust__star-img" />
        <p>
          Onze energierekening was afgelopen zomer enorm gestegen. Heel blij dat
          wij nu een goede oplossing hebben gevonden.
        </p>
        <span class="">L.J. Wood,Vinkeveen</span>
      </div>
    </div>
  </div>
</template>

<script>
import laag6 from "../assets/img/Laag 6.png";
import stars from "../assets/icons/stars.png";
import greenStars from "../assets/icons/greenStars.png";

export default {
  data() {
    return {
      laag6: laag6,
      stars: stars,
      greenStars: greenStars,
    };
  },
};
</script>

<style scoped>
.trustpilot {
  font-family: "Freizeit";
}
.trustpilot__text {
  font-size: 40px;
  line-height: 33px;
  color: #000000;
  font-weight: bold;
  font-family: "Freizeit";
  text-align: center;
}
.trustpilot__img {
  width: 15%;
  height: auto;
}
.trustpilot__cards {
  /* width: 350px; */
  /* height: 366px; */
  border-radius: 30px;
  filter: drop-shadow(6.928px -4px 27px rgba(0, 0, 0, 0.17));
  background-color: #ffffff;
}
.trust__star-img {
  height: auto;
  width: 150px;
}
</style>
