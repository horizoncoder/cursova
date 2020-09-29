<template>
  <nav>
    <div class="menu-item"><a href="#">Главная</a></div>
    <div class="menu-item"><a href="#">О нас</a></div>
    <Dropdown title="Каталог" :items="ctalog" />
    
  </nav>
</template>

<script>
import Dropdown from './Dropdown';

export default {
  name: 'navbar',
  components: {
    Dropdown
  },
  data () {
    return {
      ctalog: [
        {
          title: 'Первая',
          link: '#'
        },
        {
          title: 'Вторая',
          link:'#'
        }
      ]
    }
  }
}
</script>

<style>
nav {
  display: flex;
  align-items: center;
  justify-content: center;
}

nav .menu-item {
  color: #FFF;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;
  transition: 0.4s;
}

nav .menu-item.active,
nav .menu-item:hover {
  background-color: #444;
  border-bottom-color: #663399;
}

nav .menu-item a {
  color: inherit;
  text-decoration: none;
}
</style>