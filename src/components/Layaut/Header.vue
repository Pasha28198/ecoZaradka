<template>
  <header class="header">
    <div class="header-content">
      <div class="logo-header">
        <img :src="logo1" alt="">
      </div>
      <ul class="header-list-menu">
        <li v-for="item in menuList">
          {{item}}
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
  import logo1 from '@/assets/first.png'
  export default {
    data: () => ({
      logo1,
      menuList: [
        'special offers',
        'products',
        'contact us',
        'en'
      ],
      lang: [
        'en',
        'ru'
      ]
    })
  }
</script>

<style>
  .header {
    height: 60px;
    background-color: #026e65;
  }
  .header-content {
    padding-top: 5px;
    display: flex;
    flex-direction: row;
    width: 920px;
    margin: 0 auto;
    font-weight: 500;
    justify-content: space-between;
    cursor: pointer;
  }
  .header-list-menu {
    padding-top: 18px;
  }
  .header-list-menu li {
    text-transform: uppercase;
    color: white;
    float: left;
    margin-right: 65px;
  }
</style>

