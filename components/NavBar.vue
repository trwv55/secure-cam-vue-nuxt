<template>
  <header class="header">
    <div class="header-container container">
      <div class="header-left">
        <a href="">
          <img src="/images/header-camera.svg" alt="" />
        </a>
        <span>Secure cam</span>
      </div>
      <div class="header-right">
        <a href="tel:8(8888)888-000">8(8888)888-000</a>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style lang="scss" scoped>
.header {
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.12);
  .header-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    background-color: #fff;

    .header-left {
      display: flex;
      flex-direction: row;
      align-items: center;
      img {
        margin: 19px 14px 19px 0;
      }
      span {
        @include mon500;
        color: $colorText;
        font-size: 22px;
        line-height: 27px;
      }
    }
    .header-right {
      margin-top: 28px;
      a {
        @include mon400;
        color: #333333;
        font-size: 26px;
        line-height: 32px;
        letter-spacing: 0.25px;
      }
    }
  }
}
</style>
