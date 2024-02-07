<script>
export default {
  name: 'Header',
  data () {
    return {
        navLi: [
        {
        text: "CHARACTERS",
        link: "#",
        current: false
    },
    {
        text: "COMICS",
        link: "#",
        current: false
    },
    {
        text: "MOVIES",
        link: "#",
        current: false
    },
    {
        text: "TV",
        link: "#",
        current: false
    },
    {
        text: "GAMES",
        link: "#",
        current: false
    },
    {
        text: "COLLECTIBLES",
        link: "#",
        current: false
    },
    {
        text: "VIDEOS",
        link: "#",
        current: false
    },
    {
        text: "FANS",
        link: "#",
        current: false
    },
    {
        text: "NEWS",
        link: "#",
        current: false
    },
    {
        text: "SHOP",
        link: "#",
        current: false
    }
]
    }
  }
};
</script>

<template>
    <header>
      <div class="container">
        <img src="/img/dc-logo.png" alt="Logo_DC_Comics">
        <ul>
          <li v-for="(item, index) in navLi" :key="index" :class="{active: item.current}">
            <a :href="item.link">{{item.text}}</a>
          </li>
        </ul>
      </div>
    </header>
  </template>
  
  <style lang="scss" scoped>
  @use '../../styles/partials/variables.scss' as *;
  
  header {
    background-color: #fff;
    font-size: 15px;
    padding-top: 25px;
  
    .container {
      height: 100px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  
    img {
      height: 70%;
      padding-left: 150px;
    }
  
    ul {
      flex-grow: 1;
      text-align: right;
      line-height: 95px;
      padding-right: 70px;
  
      li {
        display: inline-block;
        font-weight: bold;
        color: $grey;
        margin: 0 10px;
        &:hover {
          cursor: pointer;
          color: $blue;
          border-bottom: 5px solid $blue;
        }
        &.active {
          color: $blue;
          border-bottom: 5px solid $blue;
        }
      }
    }
  }
  </style>