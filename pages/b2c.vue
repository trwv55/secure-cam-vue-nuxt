<template>
  <div class="app-wrapper">
    <main class="container main flex-fill">
      <StartPageCustomer />
      <WhyChooseUs />
      <MakeSave />
      <Goods />
      <Control />
      <Calculate />
      <VideoReg />
      <FindUs />
    </main>
    <Footer />
  </div>
</template>

<script>
import StartPageCustomer from "../components/StartPageCustomer.vue";
import GetConsult from "../components/GetConsult.vue";
import WhyChooseUs from "../components/WhyChooseUs.vue";
import MakeSave from "../components/MakeSave.vue";
import Goods from "../components/Goods.vue";
import Calculate from "../components/calculate/Calculate.vue";
import Control from "../components/Control.vue";
import VideoReg from "../components/VideoReg.vue";
import FindUs from "../components/FindUs.vue";
import Footer from "../components/Footer.vue";
export default {
  layout: "default",
  name: "b2c",
  components: {
    StartPageCustomer,
    WhyChooseUs,
    MakeSave,
    Goods,
    Calculate,
    Control,
    VideoReg,
    FindUs,
    Footer,
  },
};
</script>

<style lang="scss" scoped></style>
