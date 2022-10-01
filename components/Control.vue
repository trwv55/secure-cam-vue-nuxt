<template>
  <div class="control">
    <div class="container">
      <div class="control-wrapper">
        <div class="image">
          <img src="../static/images/control/phone.png" alt="" />
        </div>
        <div class="text">
          <h4>
            Контроль<br /> на расстоянии
          </h4>
          <p>
            Смотрите прямую трансляцию и записи с видеокамер,<br />
            где бы Вы не находились
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import VideoReg from "./VideoReg.vue";

export default {
  name: "Control",
};
</script>

<style lang="scss" scoped>
.control {
  position: absolute;
  left: 0;
  max-width: 1920px;
  max-height: 326px;
  width: 100%;
  height: 100%;
  background: url(/images/control/bc.png) no-repeat;
  background-size: auto auto;

  .control-wrapper {
    position: relative;
    .image {
      img {
        padding-left: 183px;
        position: absolute;
        top: -130px;
        left: 0;
      }
    }
    .text {
      padding-left: 656px;
      color: #fff;
      h4 {
        margin-top: 80px;
        font-weight: 500;
        font-size: 42px;
        line-height: 105%;
      }
      p {
        margin-top: 40px;
        font-weight: 400;
        font-size: 18px;
        line-height: 105%;
      }
    }
  }
}
</style>
