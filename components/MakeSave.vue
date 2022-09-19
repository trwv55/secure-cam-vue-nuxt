<template>
  <div class="save">
    <div class="container">
      <h3>Обезопасим каждую сферу вашей жизни</h3>
      <div class="blocks-wrapper">
        <div class="arrow arrow-left">
          <img src="../static/images/makeSave/arrow-left.svg" alt="">
        </div>
      <div class="blocks" v-for="item in blokItems" :key="item.id">
        <div class="block">
          <img :src="require(`../static/images/makeSave/${item.icon}.svg`)" alt="">
          <span>{{ item.title }}</span>
        </div>
      </div>
         <div class="arrow arrow-right">
          <img src="../static/images/makeSave/arrow-right.svg" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'MakeSave',
 data() {
  return {
    blokItems: [
      {id: 0, icon: 'office', title: 'Офисы'},
      {id: 1, icon: 'store', title: 'Магазины'},
      {id: 2, icon: 'parking', title: 'Автостоянки'},
      {id: 3, icon: 'storage', title: 'Склады'}
    ]
  }
},
};

</script>

<style lang="scss" scoped>
 .save {
   h3 {
     font-weight: 500;
    font-size: 42px;
    line-height: 51px;
   }
   .blocks-wrapper {
     display: flex;
     flex-direction: row;
     justify-content: space-between;
     margin-top: 55px;
     padding-bottom: 80px;

    .block {
        border: 2px solid rgba(229, 229, 229, 0.5);
        border-radius: 2px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        cursor: pointer;

        img {
          padding-left: 30px;
        }

        span {
          padding: 41px 83px 34px 30px;
        }
      }

    .arrow {
      img {
        width: 26px;
        height: 23px;
        color: #AAAFB4;
        margin-top: 42px;
        cursor: pointer;
      }
    
    }
   }
 }
</style>