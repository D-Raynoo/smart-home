<template>
  <div id="app" class="w-fit bg-fixed md:bg-local">
    <navBar />
    <homeSec />
    <securitySystemSec />
    <thirdSection />
    <securityModeTypeSec />
    <smartHomeSec />
    <downloadSec />
    <aboutSec />
    <whatHouseCanDoSec />
    <footerVue />
  </div>
</template>

<script>
import navBar from "./components/navBar.vue";
import homeSec from "./components/homeSec.vue";
import thirdSection from "./components/thirdSection.vue";
import securityModeTypeSec from "./components/securityModeTypeSec.vue";
import smartHomeSec from "./components/smartHomeSec.vue";
import downloadSec from "./components/downloadSec.vue";
import aboutSec from "./components/aboutSec.vue";
import whatHouseCanDoSec from "./components/whatHouseCanDoSec.vue";
import footerVue from "./components/footer.vue";
import securitySystemSec from "./components/securitySystemSec.vue";

export default {
  name: "App",
  components: {
    navBar,
    homeSec,
    thirdSection,
    securitySystemSec,
    securityModeTypeSec,
    smartHomeSec,
    downloadSec,
    aboutSec,
    whatHouseCanDoSec,
    footerVue,
  },
};
</script>

<style>
#app {
  font-family: "Montserrat", sans-serif;
  text-align: center;
  background-image: url(/public/BackgroundCompressed.jpg);
  background-size: cover;
  width: 100%;
  height: auto;
}
</style>
