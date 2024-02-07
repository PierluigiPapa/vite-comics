<script>
export default {
  name: 'MainMenu',
  data () {
    return {
      menu: [
        {
          logo: 'img/buy-comics-digital-comics.png',
          text: 'DIGITAL COMICS',
          link: '#'
        },
        
        {
          logo: 'img/buy-comics-merchandise.png',
          text: 'DC MERCHANDISE',
          link: '#'
        },
        
        {
          logo: 'img/buy-comics-subscriptions.png',
          text: 'SUBSCRIPTION',
          link: '#'
        },
        
        {
          logo: 'img/buy-comics-shop-locator.png',
          text: 'COMICS SHOP LOCATOR',
          link: '#'
        },
        
        {
          logo: 'img/buy-dc-power-visa.svg',
          text: 'DC POWER VISA',
          link: '#'
        },
      ]
    }
  }
};
</script>

<template>

<nav class="container-nav">
  <ul>
    <li v-for="element in menu">
      <a class="menu" href="">
        <div class="imgContainer"><img :src="element.logo" alt=""></div>
        <div class="text">{{ element.text }}</div>
      </a>
    </li>
  </ul>
</nav>
   
</template>
  
<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.container-nav {
  background-color: $blue-main;

  ul {
    display: flex;
    margin: auto;
    justify-content: space-around;
    max-width: 1440px;
    align-items: center;
    
    li .menu {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 50px 5px;
      
      .imgContainer {
        height: 60px;
        width: 60px;
      }
      
      img {
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
      
      .text {
        color: white;
        padding-left: 20px;
      }
      
      &:hover {
        background-color: $blue-hover;
      }
    }
  }
}
  
</style>