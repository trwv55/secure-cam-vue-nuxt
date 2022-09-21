<template>
  <div class="result">
    <div class="info">
      <p>Итого стоимость*</p>
      <h4 class="price">15 2706 ₽</h4>
      </div>

      <div class="row-wrapper">
        <div class="row">
          <span class="title">Камер</span>
          <span class="number">5 камер</span>
        </div>
         <div class="row">
          <span class="title">Время хранения</span>
          <span class="number">до 15 дней</span>
        </div>
      </div>

      <button class="result-btn">Оставить заявку</button>
      <p class="footnote">*Расчет приблизительный и не является публичным договором<br /> оферты</p>
  </div>
</template>

<script>
export default {
 name: 'Result'
}
</script>

<style lang='scss' scoped>
.result {
  background: #FFFFFF;
  box-shadow: 0px 0px 50px rgba(45, 48, 54, 0.15);
  border-radius: 2px;
  margin-left: 240px;
  position: relative;
  margin-bottom: 140px;
 .info {
   display: flex;
   flex-direction: column;
   padding: 50px 0 37px 48px;
  p {
    font-weight: 400;
    font-size: 14px;
    line-height: 17px;
    text-transform: capitalize;
    color: #AAB0BD;
    margin-bottom: 14px;
  }
  h4 {
    font-weight: 400;
    font-size: 38px;
    line-height: 46px;
    padding-right: 202px;
  }
 }
 .row-wrapper {
   display: flex;
   flex-direction: column;
   padding-left: 48px;
   margin-bottom: 42px;
   .row {
     display: flex;
     flex-direction: row;
     justify-content: space-between;
     .title {
      font-weight: 400;
      font-size: 16px;
      line-height: 20px;
      color: #AAB0BD;
      margin-top: 24px;
     }
     .number {
       font-weight: 400;
      font-size: 16px;
      line-height: 20px;
      margin-top: 24px;
      margin-right: 45px;
     }
   }
 }
 .result-btn {
  @include btn-blue;
   margin-left: 50px;
   margin-bottom: 56px;
 }
 .footnote {
   position: absolute;
   bottom: -40px;
   left: 10px;
   font-weight: 400;
   font-size: 12px;
   line-height: 15px;
   color: #8B98A7;
 }
}
</style>