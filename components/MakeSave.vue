<template>
  <div class="save">
    <div class="container">
      <h3>Обезопасим каждую сферу вашей жизни</h3>
      <div class="bloks" v-for="item in blokItems" :key="item.id">
        <div class="block">
          <img :src="require(`../static/images/makeSave/${item.icon}.svg`)" alt="">
          <span>{{ item.title }}</span>
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
      {id: 1, icon: 'office', title: 'Офисы'},
      {id: 2, icon: 'store', title: 'Магазины'}
    ]
  }
},
};

</script>

<style lang="scss" scoped>

</style>