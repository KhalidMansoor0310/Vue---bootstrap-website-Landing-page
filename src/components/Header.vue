<template>
  <div class="container-fluid header my-5">
    <div class="container">
      <div class="col-12 col-lg-10 col-md-10 m-auto">
        <h2>
          Een optimaal warm huis én bespaar tot wel
          <span class="text-success">31%</span>s op je gasverbruik
        </h2>
        <div class="row d-flex justify-content-center align-items-center">
          <div class="col-12 col-lg-6 col-md-6">
            <div class="row d-flex justify-content-center align-items-center">
              <div class="col-12 col-lg-8 col-md-8">
                <h3 class="fw-bold">De voordelen van tado°</h3>
              </div>
            </div>
            <div
              class="row d-flex justify-content-center align-items-center"
              :key="id"
              v-for="text in headerText"
            >
              <div class="col-12 col-lg-8 col-md-8 d-flex">
                <img
                  :src="tickmark"
                  class="check-img p-2 d-flex justify-content-center align-items-center"
                  alt=""
                />
                <p class="text-dark mt-1">{{ text.text }}</p>
              </div>
            </div>
            <div class="row d-flex justify-content-center align-items-center">
              <div class="col-12 col-lg-8 col-md-8">
                <button class="btn btn-lg w-100 header__btn">
                  Ja, ik wil meer informatie
                </button>
              </div>
            </div>
          </div>

          <div class="col-12 col-lg-6 col-md-6">
            <img
              src="../assets/icons/headerimg.png"
              class="header__img"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import laag8 from "../assets/img/Laag 8.png";
import tickmark from "../assets/icons/check-mark.png";

export default {
  data: function () {
    return {
      laag8: laag8,
      tickmark: tickmark,

      headerText: [
        {
          id: 1,
          text: "Bespaar tot 31% op je gasverbruik",
        },
        {
          id: 2,
          text: "Elke kamer precies de juiste temperatuur",
        },
        {
          id: 3,
          text: "Maandelijks betalen, geen grote investering",
        },
        {
          id: 4,
          text: "Na looptijd maandelijks opzegbaar",
        },
        {
          id: 5,
          text: "Installatie binnen 30 minuten geplaatst",
        },
        {
          id: 6,
          text: "Gratis support van de Nerds Helpdesk",
        },
      ],
    };
  },
};
</script>

<style scoped>
.header {
  font-family: "Ferzeit";
}
.check-img {
  height: 30px;
  width: 30px;
  /* width: 20px; */
}
.header__img {
  width: 100%;
}
.header__btn {
  border-radius: 27px;
  background-color: #f9a300;
  border: none;
  color: white;
}
</style>
