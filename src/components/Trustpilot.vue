<template>
  <div class="container trustpilot my-5">
    <div class="row">
      <img src="../assets/img/Laag 6.png" alt="" />
    </div>
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
        <img
          src="../assets/icons/greenStars.png"
          alt=""
          class="trust__star-img mb-3"
        />
        <p>
          Het werkt heel eenvoudig en fijn dat de installatie zo snel kon. Ik
          kan nu deze winter al gaan besparen op mijn energiekosten.
        </p>
        <p class="fw-bold">L.J. Wood, Vinkeveen</p>
      </div>
      <div class="col-12 col-lg-3 col-md-4 m-2 p-5 trustpilot__cards card">
        <img
          src="../assets/icons/stars.png"
          alt=""
          class="trust__star-img mb-3"
        />
        <p>
          Uitstekend geholpen door Frank. Alles was binnen 30 minuten gepiept en
          ik kon zoveel vragen stellen als ik wil.
        </p>
        <p class="fw-bold pt-4">S. Brouwer, Amerongen</p>
      </div>
      <div class="col-12 col-lg-3 col-md-4 m-2 p-5 trustpilot__cards card">
        <img
          src="../assets/icons/stars.png"
          alt=""
          class="trust__star-img mb-3"
        />
        <p>
          Onze energierekening was afgelopen zomer enorm gestegen. Heel blij dat
          wij nu een goede oplossing hebben gevonden.
        </p>
        <p class="fw-bold">W. de Vries, Driebergen</p>
      </div>
    </div>
  </div>
</template>

<script>
import laag6 from "../assets/img/Laag 6.png";

export default {
  data() {
    return {
      cardsData: [
        {
          id: 1,
          star: "../assets/icons/greenStars.png",
          text: "Het werkt heel eenvoudig en fijn dat de installatie zo snel kon. Ik kan nu deze winter al gaan besparen op mijn energiekosten.",
          name: "L.J. Wood, Vinkeveen",
        },
        {
          id: 2,
          star: "../assets/icons/stars.png",
          text: "Uitstekend geholpen door Frank. Alles was binnen 30 minuten gepiept en ik kon zoveel vragen stellen als ik wil.",
          name: "S. Brouwer, Amerongen",
        },
        {
          id: 3,
          star: "../assets/icons/stars.png",
          text: "Onze energierekening was afgelopen zomer enorm gestegen. Heel blij dat wij nu een goede oplossing hebben gevonden.",
          name: "W. de Vries, Driebergen",
        },
      ],
    };
  },
};
</script>

<style scoped>
@font-face {
  font-family: Freizeit-bold;
  src: url("../assets/fonts/Freizeit/Freizeit-Bold.otf");
}
@font-face {
  font-family: Regular;
  src: url("../assets/fonts/Freizeit/Freizeit-Regular.otf");
}

.trustpilot {
  font-family: "Freizeit";
}
.trustpilot__text {
  font-size: 24px;
  line-height: 33px;
  color: #000000;
  font-weight: bold;
  font-family: Freizeit-bold;
  text-align: center;
}
.trustpilot__img {
  width: 20%;
  height: auto;
}
@media screen and (max-width: 576px) {
  .trustpilot__img {
    width: 50%;
    height: auto;
  }
}
.trustpilot__cards {
  /* width: 350px; */
  /* height: 366px; */
  border-radius: 30px;
  filter: drop-shadow(6.928px -4px 27px rgba(0, 0, 0, 0.17));
  background-color: #ffffff;
  font-family: Regular;
}
.trust__star-img {
  height: auto;
  width: 150px;
}
</style>
