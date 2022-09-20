<template>
  <div class="main">
    <div class="overlay">
      <div class="container consult">
        <div class="links">
          <NuxtLink to="/b2c" class="nuxt-link-active">Для меня</NuxtLink>
          <NuxtLink to="/" id="active">Для бизнеса</NuxtLink>
        </div>
        <div class="title">
          <h1>
            Доверьте безопасность <br />
            Вашего бизнеса нам
          </h1>
        </div>
        <div class="text">
          <p>Оставьте заявку и получите скидку 15% на первый заказ!</p>
        </div>
        <button class="button">Получить консультацию</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GetConsult",
  components: {},
};
</script>

<style lang="scss" scoped>
.main {
  margin-bottom: 815px;
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
          color: #ffffff;
          opacity: 0.5;
        }
        #active {
          opacity: 1;
          margin-left: 61px;
          border-bottom: 1px solid #ffffff;
          padding-bottom: 4px;
        }
      }
      .title {
        margin-top: 43px;
        h1 {
          @include mon600;
          font-size: 50px;
          line-height: 105%;
          color: #ffffff;
        }
      }
      .text {
        margin-top: 52px;
        p {
          @include mon500;
          font-size: 22px;
          line-height: 105%;
          color: #ffffff;
        }
      }
      .button {
        margin-bottom: 171px;
        width: 352px;
        height: 54px;
        color: #ffffff;
        background-color: #212121;
        border: none;
        border-radius: 2px;
        margin-top: 55px;
      }
    }
  }
}
</style>
