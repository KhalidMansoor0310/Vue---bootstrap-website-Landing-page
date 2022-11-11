<template>
  <div class="container-fluid header pt-4">
    <div class="container">
      <div
        class="row d-flex justify-content-left align-items-center header__row"
      >
        <div class="col-12 col-lg-8 col-md-8 mx-auto header__left-col mb-3">
          <h4 class="header__heading">
            Een optimaal warm huis
            <span class="fw-bold text-bold"
              >én bespaar <br />
              tot wel <span class="text-success">31%</span> op je
              gasverbruik</span
            >
          </h4>
          <h3 class="header__subHeading mt-5">De voordelen van tado°</h3>
          <div class="row" :key="id" v-for="text in headerText">
            <div class="col-12 col-lg-10 col-md-10 col-sm-12 d-flex">
              <img
                :src="tickmark"
                class="check-img p-2 d-flex justify-content-end align-items-center"
                alt=""
              />
              <p class="text-dark mt-1 header__text-childerns">
                {{ text.text }}
              </p>
            </div>
          </div>
        </div>
        <div class="header__right-col">
          <img
            src="../assets/icons/headerImage.png"
            class="header__img"
            alt=""
          />
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
@font-face {
  font-family: Freizeit-bold;
  src: url("../assets/fonts/Freizeit/Freizeit-Bold.otf");
}
@font-face {
  font-family: Regular;
  src: url("../assets/fonts/Freizeit/Freizeit-Regular.otf");
}
@font-face {
  font-family: Freizeit-Medium;
  src: url("../assets/fonts/Freizeit/Freizeit-Medium.otf");
}
.header {
  font-family: "Freizeit";
  background-color: #eee;
}

.header__row {
  position: relative;
}
.header__left-col {
  /* border: 1px solid red; */
}
.text-bold {
  font-weight: 800;
}

.header__right-col img {
  position: absolute;
  top: 10%;
  left: 45%;
  width: auto;
  height: 465px;
}

/*  */

@media screen and (max-width: 882px) {
  .header__right-col img {
    top: 20%;
    left: 15%;
    width: 500px;
  }
  .header__row {
    position: relative;
  }
  .header__heading {
    position: absolute;
    top: 0%;
  }
  .header__left-col {
    margin-top: 100%;
  }
}
@media screen and (max-width: 768px) {
  .header__row {
    position: relative;
  }

  .header__left-col {
    /* position: absolute; */
    margin-top: 100%;
  }
  .header__heading h4 {
    position: absolute;
    margin-top: -100%;

    width: 100%;
    /* margin-left: -20%; */
  }
  .header__right-col img {
    top: 17%;
    left: 17%;
    width: 420px;
    height: auto;
  }
  /* .header__left-col {
    width: 270px;
    height: auto;
  } */
}
@media screen and (max-width: 512px) {
  .header__row {
    position: relative;
  }

  .header__left-col {
    /* position: absolute; */
    margin-top: 100%;
  }
  .header__heading {
    position: absolute;
    margin-top: -100%;
    font-size: 20px;
  }
  .header__right-col img {
    top: 22%;
    left: 10%;
    width: 270px;
    height: auto;
  }
}

@media screen and (max-width: 376px) {
  .header__row {
    position: relative;
  }

  .header__left-col {
    /* position: absolute; */
    margin-top: 100%;
  }
  .header__heading {
    position: absolute;
    margin-top: -100%;
    font-size: 30px !important;
  }
  .header__right-col img {
    top: 17%;
    left: 10%;
    width: 250px;
    height: auto;
  }
}

.header__heading {
  font-family: Freizeit-bold;
  /* margin-left: -20px; */
  font-size: 35px;
  margin-top: -10px;
}

.header__heading span {
  font-weight: 600;
}
.header__subHeading {
  font-family: Freizeit-bold;
}
.header__text-childerns {
  font-family: Freizeit-Medium;
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
