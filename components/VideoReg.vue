<template>
  <div class="videoReg">
    <div class="container">
      <h3>Видеорегистраторы</h3>
      <div class="blocks">
        <img src="../static/images/videoReg/chebcamera.png" alt="" />
        <img src="../static/images/videoReg/chebcamera.png" alt="" />
        <img src="../static/images/videoReg/chebcamera.png" alt="" />
        <img src="../static/images/videoReg/chebcamera.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoReg",
};
</script>

<style lang="scss" scoped>
.videoReg {
  margin-top: 520px;
  margin-bottom: 120px;
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 51px;
    letter-spacing: 0.02em;
    margin-bottom: 70px;
  }
  .blocks {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
}
</style>
