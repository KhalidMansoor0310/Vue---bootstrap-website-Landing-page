<template>
  <div class="container-fluid icons-grid py-5">
    <!-- <div class="container py-4"> -->
    <div class="col-8 m-auto">
      <h2 class="ml-2 py-2">Hoe bespaart tado°?</h2>

      <div class="row">
        <div class="col-md-6">
          <div class="row-info my-2">
            <div class="info__image-div">
              <img src="../assets/icons/location.png" class="img" alt="" />
            </div>
            <div class="info__paragraph-div">
              <p>
                Als er niemand thuis is, wordt de verwarming automatisch
                uitgezet.
              </p>
            </div>
          </div>
          <div class="row-info my-2">
            <div class="info__image-div">
              <img src="../assets/icons/window.png" class="img" alt="" />
            </div>
            <div class="info__paragraph-div">
              <p>
                Als er een raam open staat, wordt de verwarming in de ruimte
                automatisch uitgezet.
              </p>
            </div>
          </div>
          <div class="row-info my-2">
            <div class="info__image-div">
              <img src="../assets/icons/cloudy.png" class="img" alt="" />
            </div>
            <div class="info__paragraph-div">
              <p>
                Als de temperatuur buiten stijgt, past de verwarming zich tijdig
                automatisch aan.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="row-info my-2">
            <div class="info__image-div">
              <img src="../assets/icons/calender.png" class="img" alt="" />
            </div>
            <div class="info__paragraph-div">
              <p>
                Slimme verwarmingsschema’s die gebruikers zelf kunnen instellen.
              </p>
            </div>
          </div>
          <div class="row-info my-2">
            <div class="info__image-div">
              <img src="../assets/icons/remoteControl.png" class="img" alt="" />
            </div>
            <div class="info__paragraph-div">
              <p>
                SHandmatige mogelijkheid voor gebruikers om de verwarming
                tijdelijk uit of lager te zetten.
              </p>
            </div>
          </div>
          <div class="row">
            <div class="col-md-12 mt-2">
              <button class="btn btn-block btn-lg">
                Ja, ik wil meer informatie
                <i class="fa-solid fa-arrow-right py-1"></i>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- </div> -->
  </div>
</template>

<style scoped>
.icons-grid {
  background-color: #00b969;
  /* height: 579px; */
  color: white;
  font-family: Freizeit-Medium;
}
@font-face {
  font-family: Freizeit-Medium;
  src: url("../assets/fonts/Freizeit/Freizeit-Medium.otf");
}
.header {
  background-color: #eee;
}
.row-info {
  display: flex;
  justify-content: center;
  align-items: center;
}
.info__image-div {
  width: 30%;
}
.info__paragraph-div {
  width: 80%;
  /* border: 1px solid red; */
}
.fa-solid {
  color: #f9a300;
}
@media screen and (max-width: 576px) {
  .info__image-div img {
    height: 50px;
    padding: 10px;
    width: 50px;
  }
  .info__paragraph-div {
    width: 100%;
    font-size: 12px;
  }
  button {
    border-radius: 27px;
    background-color: white;
    font-size: 12px;
  }
}
p {
  color: #ffffff;
  /* font-weight: 500; */

  font-family: Freizeit-Medium;
}

.img {
  width: 66px;
  height: 66px;
  border-radius: 48px;
  background-color: #f9a300;
}
button {
  border-radius: 27px;
  background-color: white;
  width: 100%;
}
.info__icon {
  color: #f9a300;
}
</style>
