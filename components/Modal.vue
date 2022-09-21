<template>
  <div class="modal-wrapper">
    <div class="modal">
      <div class="description">
        <h4 class="modal-title">
          Видеонаблюдение для склада<br />
          помогает:
        </h4>
        <div class="blocks-text">
          <div class="row row1">
            <div class="block-text">
              <p class="title">
                Контролировать трудовую <br />дисциплину сотрудников <br />и их
                поведение
              </p>
            </div>
            <div class="block-text">
              <p class="title">
                Выявлять посторонних <br />лиц и нарушителей <br />порядка
              </p>
            </div>
          </div>
          <div class="row row2">
            <div class="block-text">
              <p class="title">
                Фиксировать воровство и<br />
                утечку служебной<br />
                информации
              </p>
            </div>
            <div class="block-text">
              <p class="title">
                Собирать доказательную<br />
                базу на случай спорных <br />ситуаций
              </p>
            </div>
          </div>
        </div>

        <div class="choose">
          <h4>Почему выбирают нас</h4>
          <div class="bloks-icons">
            <div
              class="block-icon"
              v-for="item in modalIconsItem"
              :key="item.id"
            >
              <img
                :src="require(`../static/images/chooseUs/${item.icon}.svg`)"
                alt=""
                :width="item.width"
                :height="item.height"
              />
              <p>{{ item.title }}</p>
            </div>
          </div>
        </div>
      </div>
      <div class="rotate"></div>

      <div class="form">
        <a href="/">
          <img src="../static/images/modal-close.svg" alt="" />
        </a>
        <form class="modal-form">
          <h4>
            Оставьте заявку <br />
            на подключение
          </h4>
          <div class="form-group">
            <input
              type="text"
              class="form-control"
              id="exampleInputEmail1"
              aria-describedby="emailHelp"
              placeholder="Введите имя"
            />
          </div>
          <div class="form-group">
            <input
              type="number"
              class="form-control"
              id="exampleInputPassword1"
              placeholder="Телефон"
            />
          </div>
          <div class="form-check">
            <input
              type="checkbox"
              class="form-check-input check-input"
              id="exampleCheck1"
            />
            <label class="form-check-label check-label" for="exampleCheck1"
              >Я соглашаюсь на обработку моих<br />
              персональных данных.</label
            >
          </div>
          <button type="submit" class="btn btn-primary btn-modal">
            Оставить заявку
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Modal",
  data() {
    return {
      modalIconsItem: [
        {
          id: 0,
          icon: "1",
          title: "Нет абонентской платы",
          width: "28",
          height: "28",
        },
        {
          id: 1,
          icon: "3",
          title: "Гарантия 3 года",
          width: "30",
          height: "30",
        },

        {
          id: 2,
          icon: "2",
          title: "Умный дом в Вашем смартфоне",
          width: "30",
          height: "30",
        },
        {
          id: 3,
          icon: "4",
          title: "Датчики движения и звука",
          width: "40",
          height: "40",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.modal-wrapper {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  right: 0;
  top: 0;
  left: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.6);

  .modal {
    display: flex;
    flex-direction: row;
    box-shadow: 0px 4px 40px rgba(0, 0, 0, 0.1);
    background: #fff;
    z-index: 1;
    border-radius: 4px;
    color: #2d3036;
    position: fixed;
    // top: 50px;
    // width: 905px;
    // height: 470px;
    margin: 0 auto;

    .description {
      padding-top: 50px;
      padding-bottom: 50px;
      padding-left: 40px;
      .modal-title {
        font-weight: 500;
        font-size: 20px;
        line-height: 24px;
        margin-bottom: 25px;
      }
      .blocks-text {
        display: flex;
        flex-direction: row;

        .block-text {
          font-weight: 400;
          font-size: 15px;
          line-height: 18px;
          margin-right: 8px;
          margin-bottom: 8px;
          box-shadow: 0px 4px 40px rgba(0, 0, 0, 0.1);
          border-radius: 4px;
          border: 1px solid #aab0bd;
          padding: 12px;
        }
      }
      .choose {
        width: 480px;
        padding-right: 22px;
        h4 {
          font-weight: 500;
          font-size: 18px;
          line-height: 22px;
        }
        .bloks-icons {
          display: flex;
          flex-direction: row;
          justify-content: space-between;
          margin-top: 12px;
          .block-icon {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;

            p {
              font-size: 13px;
              line-height: 15px;
              text-align: center;
            }
          }
        }
      }
    }
    .rotate {
      content: "";
      border: 1px solid #f2f2f2;
    }

    .form {
      img {
        float: right;
        margin-top: 29px;
        margin-right: 25px;
      }
      .modal-form {
        padding-left: 21px;
        h4 {
          padding: 50px 0 25px 0;
          font-weight: 500;
          font-size: 21px;
          line-height: 26px;
        }
        .form-group {
          // margin-left: 21px;
          margin-right: 40px;
          margin-bottom: 12px;
          input {
            border: 1px solid #aab0bd;
            filter: drop-shadow(0px 4px 13px rgba(0, 0, 0, 0.1));
            border-radius: 3px;
            font-weight: 400;
            font-size: 14px;
            line-height: 17px;
            padding: 13px 158px 12px 12px;
          }
        }
        .form-check {
          display: flex;
          flex-direction: row;
          margin-top: 20px;
          .check-input {
            border: 1px solid #aab0bd;
            border-radius: 3px;
            width: 22px;
            height: 22px;
          }
          .check-label {
            font-weight: 400;
            font-size: 14px;
            line-height: 17px;
            margin-left: 8px;
            color: #aab0bd;
          }
        }
        .btn-modal {
          @include btn-blue;
          width: 305px;
          height: 48px;
          margin-top: 20px;
          margin-right: 40px;
        }
      }
    }
  }
}
</style>
