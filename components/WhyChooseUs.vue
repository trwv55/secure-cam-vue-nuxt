<template>
  <div class="container choose">
    <h3>Почему выбирают именно нас</h3>
    <p class="choose-par">
      Качество, надежность и безопасность - наши главные приоритеты.
    </p>
    <div class="icons">
      <div class="col">
        <img src="/images/chooseUs/1.svg" alt="" />
        <p class="icons-text">Нет абонентской платы</p>
      </div>
      <div class="col">
        <img src="/images/chooseUs/2.svg" alt="" />
        <p class="icons-text">Умный дом в Вашем смартфоне</p>
      </div>
      <div class="col">
        <img src="/images/chooseUs/3.svg" alt="" />
        <p class="icons-text">Гарантия 3 года</p>
      </div>
      <div class="col">
        <img src="/images/chooseUs/4.svg" alt="" />
        <p class="icons-text">Датчики движения и звука</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WhyChooseUs",
};
</script>

<style lang="scss" scoped>
.choose {
  padding-bottom: 120px;
  @media screen and (max-width: 500px) {
    padding-bottom: 80px;
  }
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 51px;
    color: $colorText;

    @media screen and (max-width: 500px) {
      font-size: 22px;
    }
  }
  p {
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    margin-top: 30px;
    color: $colorText;
  }

  .choose-par {
    @media screen and (max-width: 500px) {
      display: none;
    }
  }
  .icons {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 41.4px;

    @media screen and (max-width: 500px) {
      flex-direction: column;
    }
    .col {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;

      img {
        @media screen and (max-width: 500px) {
          width: 50px;
        }
      }

      @media screen and (max-width: 500px) {
        flex-direction: row;
        justify-content: flex-start;
        align-items: center;
        margin-bottom: 15px;
      }
      .icons-text {
        font-weight: 400;
        font-size: 22px;
        line-height: 26px;
        text-align: center;

        @media screen and (max-width: 500px) {
          font-size: 18px;
          line-height: 21px;
          padding-left: 30px;
        }
      }
    }
  }
}
</style>
