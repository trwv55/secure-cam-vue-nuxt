<template>
  <div class="container consult">
    <div class="consult-left">
      <div class="links">
        <NuxtLink to="/b2c" id="active">Для меня</NuxtLink>
        <NuxtLink to="/">Для бизнеса</NuxtLink>
      </div>

      <h1>
        Умное видеонаблюдение <br />
        уже в вашем доме
      </h1>

      <div class="text">
        <p>Оставьте заявку и получите скидку 15% на первый заказ!</p>
      </div>
      <button class="button">Получить консультацию</button>
    </div>
    <div class="consult-right">
      <img
        src="../static/images/customer.png"
        alt=""
        width="600"
        height="450"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "StartPageCustomer",
};
</script>

<style lang="scss" scoped>
.consult {
  display: flex;
  flex-direction: row;
  margin-bottom: 165px;

  @media screen and (max-width: 500px) {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 80px;
  }
  .consult-left {
    .links {
      padding-top: 122px;
      padding-bottom: 58px;

      @media screen and (max-width: 500px) {
        padding-top: 40px;
      }
      a {
        font-weight: 400;
        font-size: 22px;
        line-height: 105%;
        color: rgba(0, 0, 0, 0.5);
        margin-right: 62px;

        @media screen and (max-width: 500px) {
          font-size: 18px;
        }
      }
      #active {
        color: #0b1b28;
        border-bottom: 1px solid #5082f4;
        padding-bottom: 4px;
      }
    }
    h1 {
      font-weight: 600;
      font-size: 50px;
      line-height: 105%;

      @media screen and (max-width: 500px) {
        font-size: 32px;
        line-height: 110%;
      }
    }
    .text > p {
      font-weight: 500;
      font-size: 22px;
      line-height: 105%;
      margin-top: 56px;
      margin-bottom: 56px;

      @media screen and (max-width: 500px) {
        font-size: 16px;
        margin-top: 30px;
        margin-bottom: 0;
      }
    }
    .button {
      width: 325px;
      height: 54px;
      background: #5082f4;
      border-radius: 2px;
      color: #fff;
      border: none;
      cursor: pointer;
      @media screen and (max-width: 500px) {
        margin-top: 30px;
        width: 345px;
        height: 48px;
      }
    }
  }
  .consult-right {
    margin-top: 103px;
    @media screen and (max-width: 500px) {
      margin-top: 30px;
    }
  }
}
</style>
