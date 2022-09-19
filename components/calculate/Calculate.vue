<template>
  <div class="calculate">
    <div class="container">
      <h3>Рассчитайте стоимость видеонаблюдения</h3>
      <p>Никаких тарифов и абонентских плат - платите один раз и пользуйтесь камерой.</p>
      <div class="form-wrapper">
<div class="checkbox-form">

  <div class="checkbox-wrapper">
    <div class="form-check checkbox">
  <input class="form-check-input input" type="checkbox" value="" id="flexCheckDefault">
  <label class="form-check-label label" for="flexCheckDefault">
    Монтаж
  </label>
</div>
<div class="form-check checkbox">
  <input class="form-check-input input" type="checkbox" value="" id="flexCheckChecked" checked>
  <label class="form-check-label label" for="flexCheckChecked">
    Full HD камера
  </label>
</div>
    </div>
      <Form />
</div>
      <Result />
      </div>
    </div>
  </div>
</template>

<script>
import Form from './Form.vue';
import Result from './Result.vue';

export default {
  name: 'Calculate',
  components: {
    Form, Result
  } 
}
</script>

<style lang="scss" scoped>
.calculate {
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 120%;
  }
  p {
    font-weight: 500;
    font-size: 24px;
    line-height: 29px;
    margin-top: 30px;
    margin-bottom: 50px;
    color: #5082F4;
  }
  .form-wrapper {
    display: flex;
    flex-direction: row;
    .checkbox-form {
      .checkbox-wrapper {
        display: flex;
        flex-direction: row;
        padding-bottom: 47px;
        .checkbox {
          margin-right: 50px;
          display: flex;
          flex-direction: row;
          align-items: center;
          .input {
            width: 24px;
            height: 24px;
            border: 1px solid #AAB0BD;
            border-radius: 3px;
            margin-right: 10px;
          }
          .label {
            font-weight: 400;
            font-size: 20px;
            line-height: 100%;
            color: #333333;
          }
        }
      }
    }
  }
}
</style>