<template>
  <div class="app-wrapper">
    <main class="main container flex-fill">
      <GetConsult />
      <WhyChooseUs />
      <MakeSave />
      <Goods />
      <Clients />
      <Calculate />
      <Control />
      <VideoReg />
      <FindUs />
    </main>
    <Footer />
  </div>
</template>

<script>
import GetConsult from "../components/GetConsult.vue";
import WhyChooseUs from "../components/WhyChooseUs.vue";
import MakeSave from "../components/MakeSave.vue";
import Goods from "../components/Goods.vue";
import Clients from "../components/Clients.vue";
import Calculate from "../components/calculate/Calculate.vue";
import Control from "../components/Control.vue";
import VideoReg from "../components/VideoReg.vue";
import FindUs from "../components/FindUs.vue";
import Footer from "../components/Footer.vue";


export default {
  layout: "default",
  name: "IndexPage",
  components: {
    GetConsult,
    WhyChooseUs,
    MakeSave,
    Goods,
    Clients,
    Calculate,
    Control,
    VideoReg,
    FindUs,
    Footer,
  },
};
</script>

<style lang="scss"></style>
