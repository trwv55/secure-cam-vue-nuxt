<template>
<div class="main">
  <div class="overlay">
  <div class="container consult">
    <div class="links">
      <a href="">Для меня</a>
      <a id="active" href="">Для бизнеса</a>
    </div>
    <div class="title">
      <h1>Доверьте безопасность <br /> Вашего бизнеса нам</h1>
    </div>
    <div class="text">
      <p>Оставьте заявку и получите скидку 15% на первый заказ!</p>
    </div>
    <button class="button">Получить консультацию</button>
  </div>
  <WhyChooseUs/>
  <MakeSave />
  </div>

 </div>


</template>

<script>
import WhyChooseUs from './WhyChooseUs.vue';
import MakeSave from './MakeSave.vue';
export default {
  
  name: 'GetConsult',
  components: {
    WhyChooseUs, MakeSave
  } 
};
</script>

<style lang="scss" scoped>
.main {
.overlay {
  position: absolute;
  left: 0;
  max-height: 693px;
  max-width: 1921px;
  height: 100%;
  width: 100%;
  background: url(/images/bc-b2b.png) no-repeat;
  background-size: auto auto;
  .consult {
    margin-bottom: 120px;
    .links {
      padding-top: 168px;
       a {
        @include mon500;
        font-size: 22px;
        line-height: 105%;
        color: #FFFFFF;
        opacity: 0.5;
      }
       #active {
          opacity: 1;
          margin-left: 61px;
          border-bottom: 1px solid #FFFFFF;
          padding-bottom: 4px;  
        }
    }
    .title {
      margin-top: 43px;
      h1 {
        @include mon600;
        font-size: 50px;
        line-height: 105%;
        color: #FFFFFF;
      }
    }
    .text {
      margin-top: 52px;
      p {
        @include mon500;
        font-size: 22px;
        line-height: 105%;
        color: #FFFFFF;
      }
    }
    .button {
      margin-bottom: 171px;
      width: 352px;
      height: 54px;
      color: #FFFFFF;
      background-color: #212121;
      border: none;
      border-radius: 2px;
      margin-top: 55px;
    }
  }
}
}

</style>