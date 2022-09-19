<template>
      <form>
  <div class="form-group">
    <label class="form-label" for="exampleInputEmail1">Количество камер</label>
    <div class="wrapper">
  <input type="number" class="form-control form-input" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="4">
    </div>
    <span>1 камера</span>
  
    
  </div>
  <div class="form-group">
    <label class="form-label" for="exampleInputPassword1">Время хранения</label>
    <div class="wrapper">
   <input type="number" class="form-control form-input" id="exampleInputPassword1" placeholder="15">
    </div>
    <span>до 10 дней</span>
 
  </div>
</form>
</template>

<script>
export default {
 name: 'Form'
}
</script>

<style lang="scss" scoped>
.form-group {
  display: flex;
  flex-direction: column;
  padding-bottom: 65px;
  .form-label {
    font-weight: 400;
    font-size: 18px;
    line-height: 22px;
    margin-bottom: 10px;
    color: #333333;
  }
  .wrapper {
    display: flex;
    flex-direction: row;
    align-items: center;
    .form-input {
      padding-left: 25px;
      font-weight: 400;
      font-size: 18px;
      line-height: 22px;
      color: #333333;
      width: 599px;
      height: 62px;
      border: 2px solid #AAB0BD;
      border-radius: 4px;
    }
  }
   span {
      display: inline-block;
      font-weight: 400;
      font-size: 14px;
      line-height: 17px;
      margin-top: 5px;
      color: #70747E;

    }
}
</style>