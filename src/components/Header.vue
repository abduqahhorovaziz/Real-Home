<template>
  <div class="hello">
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container"> 
        <a class="navbar-brand logo" href="/"><img src="../assets/images/logo.png" alt="logo"></a>
        <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li
              class="nav-item active menu-link"
              v-for="(menu, index) in headerMenuList"
              :key="index"
            >
              <router-link class="nav-link " :to="menu.path">
                {{ menu.name }}
              </router-link>
            </li>
          </ul>
          <div class="icons">
            <a href="https://www.facebook.com/" target="_blank"><i class="fa-brands fa-facebook-f"></i></a>
            <a href="https://www.pinterest.com/" target="_blank"><i class="fa-brands fa-pinterest"></i></a>
            <a href="https://www.instagram.com/" target="_blank"><i class="fa-brands fa-instagram"></i></a>
            <a href="https://www.myaccount.google.com/" target="_blank"><i class="fa-brands fa-google-plus-g"></i></a>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
import {menuList} from '../constants/menuLinks.js'
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: menuList,
    };
  },
};
</script>

<style lang="scss">
@import '../assets/layouts/index';

.container{
  max-width: 1240px;
}
.navbar{
  height: 90px;
}
.navbar-nav{
  height: 90px;
}
.logo{
  padding-right: 180px;
}

.collapse-fontsize{
  font-size: 18px;
}

.menu-link{
  padding: 25px;

  &:hover{
    background-color: $gray;
  }
}

.icons{
  a{
    width: 30px;
    height: 30px;
    border: 1px solid $gray;
    text-align: center;
    border-radius: 50%;
    margin-right: 10px;
    display: inline-block;
    
    i{
      color: black;
    }
  }
}

</style>
