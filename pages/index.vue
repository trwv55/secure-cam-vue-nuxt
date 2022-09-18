<template>
  <div class="app-wrapper">
    <main container main flex-fill >
        <GetConsult />
    </main> 
  </div>
</template>


<script>
import GetConsult from '../components/GetConsult.vue';

export default {
  layout: 'default',
  name: 'IndexPage',
  components: { GetConsult },
};
</script>

<style lang="scss">

</style>
