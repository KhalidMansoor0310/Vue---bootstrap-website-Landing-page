<template>
  <div class="container-fluid icons-grid py-5">
    <div class="container">
      <div class="col-6">
        <h2 class="ml-2">Hoe bespaart tado°?</h2>
      </div>
    </div>
    <div class="container py-4">
      <div class="row">
        <div
          class="col-12 col-lg-6 col-md-6"
          :key="info.id"
          v-for="info in info"
        >
          <div class="row d-flex justify-content-center align-items-center">
            <div class="col-12 col-lg-2 col-md-2 my-2">
              <img :src="info.source" alt="" />
            </div>
            <div class="col-12 col-lg-5 col-md-5">
              <p>
                {{ info.text }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import location from "../assets/icons/location.png";
import window from "../assets/icons/window.png";
import cloudy from "../assets/icons/cloudy.png";
import remoteControl from "../assets/icons/remoteControl.png";
import calender from "../assets/icons/calender.png";

export default {
  data: function () {
    return {
      info: [
        {
          id: 1,
          text: "Als er niemand thuis is, wordt de verwarming automatisch uitgez",
          source: location,
        },
        {
          id: 2,
          text: "Als er een raam open staat, wordt de verwarming in de ruimte au",
          source: window,
        },
        {
          id: 3,
          text: "Als de temperatuur buiten stijgt, past de verwarming zich tijdi",
          source: cloudy,
        },
        {
          id: 4,
          text: "Slimme verwarmingsschema’s die gebruikers zelf kunnen instellen",
          source: calender,
        },
        {
          id: 5,
          text: "Handmatige mogelijkheid voor gebruikers om de verwarming tijdel",
          source: remoteControl,
        },
      ],
    };
  },
};
</script>

<style scoped>
.icons-grid {
  background-color: #00b969;
  /* height: 579px; */
  color: white;
}
.header {
  background-color: #eee;
}

p {
  color: #ffffff;
  font-weight: 500;
  font-family: "Freizeit";
}

.img {
  width: 96px;
  height: 96px;
  border-radius: 48px;
  background-color: #f9a300;
}
button {
  /* width: 400px;
    height: 53px; */
  border-radius: 27px;
}
</style>
