<template>
  <div class="container choose">
    <h3>Почему выбирают именно нас</h3>
    <p>Качество, надежность и безопасность - наши главные приоритеты. </p>
    <div class="icons">
        <div class="col">
          <img src="/images/chooseUs/1.svg" alt="">
          <p>Нет абонентской<br /> платы</p>
        </div>
        <div class="col">
          <img  src="/images/chooseUs/2.svg" alt="">
          <p>Умный дом<br /> в Вашем смартфоне</p>
        </div>
        <div class="col">
          <img src="/images/chooseUs/3.svg" alt="">
          <p>Гарантия <br />3 года</p>
        </div>
        <div class="col">
          <img src="/images/chooseUs/4.svg" alt="">
          <p>Датчики движения <br />и звука</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'WhyChooseUs',
};

</script>

<style lang="scss" scoped>
 .choose {
    padding-bottom: 120px;
    h3 {
      font-weight: 500;
      font-size: 42px;
      line-height: 51px;
      color: $colorText;
    }
    p {
      font-weight: 400;
      font-size: 24px;
      line-height: 29px;
      margin-top: 30px;
      color: $colorText;
    }
    .icons {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      margin-top: 41.4px;
      .col {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        p {
          font-weight: 400;
          font-size: 22px;
          line-height: 26px;
          text-align: center;
        }

      }

    }
 }
</style>