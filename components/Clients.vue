<template>
  <div class="clients">
    <div class="container">
      <h3>Нам доверяют уже более 8 лет</h3>
      <p>Наши клиенты уверены в нас и наших услугах.</p>
      <div class="wrapper">
        <div class="clients-blocks" v-for="item in clientsItems" :key="item.id">
        <div class="block">
          <img :src="require(`../static/images/clients/${item.icon}.png`)" alt="">
          <span>{{ item.title }}</span>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'Clients',
 data() {
   return {
     clientsItems: [
        {id: 0, icon: 'logo 1', title: 'Минобороны России'},
         {id: 1, icon: 'logo 2', title: 'Минюст ЧР'},  
          {id: 2, icon: 'logo 3', title: 'Группа “Т Плюс”'},
           {id: 3, icon: 'logo 4', title: 'Прокуратура ЧР'},
            {id: 4, icon: 'logo 5', title: 'ПАО “Ростелеком”'},
            {id: 5, icon: 'logo 6', title: 'ПАО “Транснефть”'},
             {id: 6, icon: 'logo 7', title: 'АО “АККОНД”'},
              {id: 7, icon: 'logo 8', title: 'ООО “Аркто”'},
                {id: 8, icon: 'logo 9', title: 'АО “Электрощит”'},
                 {id: 9, icon: 'logo 10', title: 'ПАО “Газпром”'},
     ]
   }
 }
}
</script>

<style lang="scss" scoped>
.clients {
  h3 {
    font-weight: 500;
    font-size: 42px;
    line-height: 120%;
  }
  p {
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    margin-top: 30px;
    margin-bottom: 60px;
  }
  .wrapper {
  .clients-blocks {
    display: inline-block;
    .block {
      display: flex;
      flex-direction: column;
      align-items: center;
      flex-grow: 1;
      width: 200px;
      height: 145px;
      cursor: pointer;
      margin-bottom: 44px;
      margin-right: 51px;
       
    span {
      margin-top: 20px;
    }
    }
  }

  }

}
</style>