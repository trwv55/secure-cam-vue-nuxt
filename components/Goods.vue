<template>
  <div class="goods">
    <div class="container">
      <h3>Камеры видеонаблюдения</h3>
      <div class="links">
        <a class="active" href="#">Внутренние</a>
        <a href="#">Уличные</a>
      </div>
      <div class="image">
        <img src="../static/images/goods/offer.png" alt="" />
      </div>

      <div class="blocks-wrapper">
        <div class="arrow arrow-left">
          <img src="../static/images/makeSave/arrow-left.svg" alt="" />
        </div>
        <div class="blocks" v-for="item in blokGoodsItems" :key="item.id">
          <div class="block">
            <img
              :src="require(`../static/images/goods/${item.icon}.png`)"
              alt=""
            />
            <div class="block-info">
              <h5 class="title">{{ item.title }}</h5>
              <h5 class="decs">{{ item.desc }}</h5>
              <span>{{ item.span }}</span>
              <h4 class="price">{{ item.price }}</h4>
            </div>
          </div>
        </div>
        <div class="arrow arrow-right">
          <img src="../static/images/makeSave/arrow-right.svg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Goods",
  data() {
    return {
      blokGoodsItems: [
        {
          id: 0,
          icon: "C1C PIR",
          title: "C1C PIR",
          desc: "IP-видеокамера",
          span: "EZVIZ",
          price: "5 990 P",
        },
        {
          id: 1,
          icon: "C2C 1080P",
          title: "C2C 1080P",
          desc: "IP-видеокамера",
          span: "EZVIZ",
          price: "5 699 P",
        },
        {
          id: 2,
          icon: "DS-T204 (2.8mm)",
          title: "DS-T204 (2.8mm)",
          desc: "HD-TVI видеокамера",
          span: "HiWatch",
          price: "4 630 P",
        },
        {
          id: 3,
          icon: "IPC-D42P-0280B-IMOU",
          title: "IPC-D42P-0280B-IMOU",
          desc: "IP-видеокамера",
          span: "IMOU",
          price: "8 690 P",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.goods {
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 120%;

    @media screen and (max-width: 500px) {
      font-size: 22px;
      line-height: 24px;
    }
  }
  .links {
    margin-top: 40px;
    @media screen and (max-width: 500px) {
      margin-top: 30px;
    }
    a {
      color: #c4c4c4;
      font-weight: 400;
      font-size: 14px;
      line-height: 17px;
      margin-right: 30px;
      @media screen and (max-width: 500px) {
        font-size: 18px;
        line-height: 105%;
        margin-right: 24px;
      }
    }
    .active {
      letter-spacing: 0.05px;
      color: #0b1b28;
      border-bottom: 1px solid #5082f4;
      padding-bottom: 5px;
    }
  }
  .image {
    margin: 50px 124px 40px;
    @media screen and (max-width: 500px) {
      margin-left: 0;
      margin-right: 0;
    }
  }

  .blocks-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 40px;
    padding-bottom: 120px;
    .block {
      border: 2px solid rgba(229, 229, 229, 0.5);
      border-radius: 2px;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      img {
        padding-left: 23px;
        width: 90px;
        height: 90px;
      }
      .block-info {
        padding: 20px 59px 20px 15px;
        .title,
        .decs {
          font-weight: 400;
          font-size: 12px;
          line-height: 150.4%;
        }
        span {
          margin-top: 8px;
          margin-bottom: 8px;
          font-weight: 400;
          font-size: 10px;
          line-height: 150.4%;
          color: #989898;
        }
        .price {
          font-weight: 500;
          font-size: 20px;
          line-height: 150.4%;
        }
      }
    }

    .arrow {
      img {
        width: 26px;
        height: 23px;
        color: #aaafb4;
        margin-top: 58px;
        cursor: pointer;
      }
    }
  }
}
</style>
