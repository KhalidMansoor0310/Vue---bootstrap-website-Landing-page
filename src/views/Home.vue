<template>
  <div>
    <Header />
    <Information />
    <Laagf />
    <Trustpilot />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import location from "../assets/icons/location.png";
import tickmark from "../assets/icons/check-mark.png";
import Header from "../components/Header.vue";
import laag8 from "../assets/img/Laag 8.png";
import Laagf from "../components/Laagf.vue";
import Trustpilot from "../components/Trustpilot.vue";
import Footer from "../components/Footer.vue";
import Information from "../components/Information.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    Laagf,
    Trustpilot,
    Footer,
    Header,
    Information,
  },
  data: function () {
    return {
      location: location,
      laag8: laag8,
      tickmark: tickmark,
    };
  },
};
</script>
