<template>
  <main-container class="app-wrapper">
    <template v-slot:header>
     <NavBar />  
    </template>
    <main >
        <GetConsult />
        <WhyChooseUs />
    </main> 
 <template v-slot:footer>
     <Footer />
  </template>
  </main-container>
</template>

<script>
import NavBar from '../components/NavBar.vue';
import MainContainer from '../components/MainContainer.vue';
import GetConsult from '../components/GetConsult.vue';
import Footer from '../components/Footer.vue';
import WhyChooseUs from '../components/WhyChooseUs.vue';

export default {
  name: 'IndexPage',
  components: { NavBar, GetConsult, WhyChooseUs, Footer, MainContainer},
};
</script>

<style lang="scss">

</style>
