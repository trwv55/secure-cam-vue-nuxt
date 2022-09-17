<template>
  <div class="app-wrapper">
    <header class="container">
      <NavBar />
    </header>
    <main class="container main">
        <GetConsult />
    </main> 
   
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue';
import GetConsult from '../components/GetConsult.vue';
// import WhyChooseUs from '../components/WhyChooseUs.vue';

export default {
  name: 'IndexPage',
  components: { NavBar, GetConsult, },
};
</script>

<style lang="scss">

</style>
