<template>
  <footer class="footer">
    <div class="container">
      <div class="row-wrapper">
        <div class="col col1">
          <img src="images/footer-socials.svg" alt="" />
          <p class="note">
            Продолжая использовать наш сайт, вы даете <br />
            согласие на обработку файлов Cookies и других <br />
            пользовательских данных, в соответствии с <br /><span id="padding"
              >Политикой конфиденциальности.</span
            >
          </p>
        </div>
        <div class="col-wrapper">
          <div class="col col2">
            <a class="row1 number" href="tel:8(8888)888-000">8(8888)888-000</a>
            <p class="row2 phone">телефон</p>
            <a class="row3 video" href="#">Видеонаблюдение</a>
            <a class="row4 fire" href="#">Пожарная сигнализация</a>
          </div>
          <div class="col col3">
            <a href="mailto:info@camera11.ru" class="row1 mail"
              >info@camera11.ru</a
            >
            <p class="row2 post">почта</p>
            <a href="#" class="row3 domof">Домофония</a>
            <a href="#" class="row4 save">Безопасный дом</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
.footer {
  margin-top: 85px;
  background-color: #202427;
  padding-bottom: 180px;
  .row-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    flex-grow: 2 1;
    padding-top: 65px;
    padding-bottom: 83px;
    border-bottom: 1px solid #36393c;

    .col {
      color: #fff;
      .note {
        font-weight: 400;
        font-size: 12px;
        line-height: 161%;
        color: #d2d3d4;
        margin-top: 21px;
        #padding {
          border-bottom: 1px solid #5082f4;
        }
      }
      .row1 {
        font-weight: 400;
        font-size: 20px;
        line-height: 24px;
      }
      .row2 {
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        margin-top: 9px;
        color: #d2d3d4;
      }

      .row3,
      .row4 {
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
      }
      .row3 {
        margin-top: 59px;
        margin-bottom: 23px;
      }
    }
    .col-wrapper {
      display: flex;
      flex-direction: row;
      .col2 {
        margin-right: 141px;
        a {
          color: #fff;
        }
      }
      .col2,
      .col3 {
        display: flex;
        flex-direction: column;
        margin-top: 15px;
      }
      .col3 {
        margin-right: 120px;
        a {
          color: #fff;
        }
      }
    }
  }
}
</style>
