<template>
  <div class="find">
    <div class="container">
      <div class="wrapper">
        <div class="info">
          <h3>Как нас найти</h3>
          <div class="office">
            <h5 class="main-office">Главный офис</h5>
            <p class="city">г. Москва,ул. Калинина, 7</p>
            <a href="tel:8(8888)888-000">8(8888)888-000</a>
            <p class="time">пн-пт. 09:00 - 18:00</p>
            <p class="close">cб-вс. выходной</p>
          </div>
          <div class="office">
            <h5 class="sell-office">Офис продаж</h5>
            <p class="city">г. Москва,ул. Калинина, 7</p>
            <a href="tel:8(8888)888-000">8(8888)888-000</a>
            <p class="time">пн-пт. 09:00 - 18:00</p>
            <p class="close">cб-вс. выходной</p>
          </div>
          <a class="quest" href="#">Как пройти до торговой точки</a>
        </div>
        <div class="map">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1043.1136615639416!2d37.365126392359976!3d55.7055271644107!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46b54e49571b3905%3A0x9eea5621a367dbc5!2z0YPQuy4g0JrQsNC70LjQvdC40L3QsCwgMTQzMDI2!5e0!3m2!1sru!2sru!4v1663661928292!5m2!1sru!2sru"
            width="600"
            height="450"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Findus",
};
</script>

<style lang="scss" scoped>
.find {
  padding-bottom: 80px;
  .wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    .info {
      h3 {
        font-weight: 400;
        font-size: 46px;
        line-height: 56px;
        margin-bottom: 43px;
      }
      .office {
        h5 {
          font-weight: 600;
          font-size: 19px;
          line-height: 26px;
          margin-bottom: 15px;
        }
        .main-office {
          &::before {
            content: url(../static/images/findUs/main-office.svg);
            padding-right: 6px;
          }
        }
        p,
        a {
          font-weight: 400;
          font-size: 16px;
          line-height: 22px;
          color: #474b59;
        }
        .city {
          margin-bottom: 6px;
          &::before {
            content: url(../static/images/findUs/city.svg);
            padding-right: 6px;
          }
        }
        a {
          margin-bottom: 6px;
          &::before {
            content: url(../static/images/findUs/tel.svg);
            padding-right: 6px;
          }
        }
        .time {
          margin-top: 6px;
          &::before {
            content: url(../static/images/findUs/time.svg);
            padding-right: 6px;
          }
        }
        .close {
          font-weight: 400;
          font-size: 14px;
          line-height: 19px;
          color: rgba(71, 75, 89, 0.8);
          padding-left: 16px;
        }
        .sell-office {
          margin-top: 45px;
          &::before {
            content: url(../static/images/findUs/sell-of.svg);
            padding-right: 6px;
          }
        }
      }
      .quest {
        margin-top: 18px;
        font-weight: 400;
        font-size: 16px;
        line-height: 22px;
        margin-top: 18px;
        color: #0b1b28;
        border-bottom: 1px solid #5082f4;
        padding-bottom: 4px;
      }
    }
    .map {
      margin-right: 80px;
    }
  }
}
</style>
