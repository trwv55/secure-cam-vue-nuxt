<template>
  <div class="save">
    <div class="container">
      <h3>Обезопасим каждую сферу вашей жизни</h3>
      <div class="blocks-wrapper">
         <client-only>
         <carousel        
          class="blocks" 
          v-bind="options">
          <slide 
            v-for="item in blokItems" 
            :key="item.id" 
            class="block">
             <img
              :src="require(`../static/images/makeSave/${item.icon}.svg`)"
              alt=""
            />
            <span>{{ item.title }}</span>
           </slide>
     
         </carousel>
          </client-only>
     </div>




      
      <!-- <div class="blocks-wrapper">
        <div class="arrow arrow-left">
          <img src="../static/images/makeSave/arrow-left.svg" alt="" />
        </div>

        <div class="blocks" v-for="item in blokItems" :key="item.id">
          <div class="block">
            <img
              :src="require(`../static/images/makeSave/${item.icon}.svg`)"
              alt=""
            />
            <span>{{ item.title }}</span>
          </div>
        </div> -->

        <!-- <div class="arrow arrow-right">
          <img src="../static/images/makeSave/arrow-right.svg" alt="" />
        </div> -->

      </div>
    </div>

</template>

<script>
export default {
  name: "MakeSave",
  components: {  },
  data() {
    return {
      blokItems: [
        { id: 0, icon: "office", title: "Офисы" },
        { id: 1, icon: "store", title: "Магазины" },
        { id: 2, icon: "parking", title: "Автостоянки" },
        { id: 3, icon: "storage", title: "Склады" },
      ],
      options: {
        loop: true,
        perPage: 3,
        paginationEnabled: false,
        arrows: true,
        navigationEnabled: true,
        navigationNextLabel: "<button class='rightnav'><keyboard_arrow_right></button>"
      }
     
    }
  }

};
</script>

<style lang="scss" scoped>
.save {
 
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 51px;

    @media screen and (max-width: 500px) {
      font-size: 22px;
      line-height: 24px;
    }
  }
  .blocks-wrapper {
    // display: flex;
    // flex-direction: row;
    // justify-content: space-between;
    margin-top: 55px;
    padding-bottom: 80px;

    @media screen and (max-width: 500px) {
      margin-top: 30px;
      flex-wrap: wrap;
      max-width: 500px;
      justify-content: flex-start;
    }

    .block {
      border: 2px solid rgba(229, 229, 229, 0.5);
      border-radius: 2px;
      // display: flex;
      // flex-direction: row;
      // justify-content: center;
      cursor: pointer;

      @media screen and (max-width: 500px) {
        flex-direction: column;
        align-items: center;
        width: 167px;
        height: 130px;
        margin: 10px;
      }

      img {
        padding-left: 30px;

        @media screen and (max-width: 500px) {
          width: 50px;
          height: 50px;
          padding-left: 0;
        }
      }

      span {
        padding: 41px 83px 34px 30px;

        @media screen and (max-width: 500px) {
          padding: 12px 53px 17px 53px;
        }
      }
    }

    .arrow {
      @media screen and (max-width: 500px) {
        display: none;
      }

      img {
        width: 26px;
        height: 23px;
        color: #aaafb4;
        margin-top: 42px;
        cursor: pointer;
      }
    }
  }
}
</style>
