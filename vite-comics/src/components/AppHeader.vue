<template>
    <header class="header">
      <div class="container">

        <nav class="header-menu">
            <img class="logo" src="../../public/dc-logo.png" alt="">

          <ul class="menu-list">

            <li class="header-list-items" v-for="(item, index) in menuList" :key="index">
                <a :href="item.link">
                    {{item.label}}
                </a>
            </li>
            <!-- <li class="menu-item active">
                <a href="#">Comics</a>
            </li>
            <li>
                <a href="#">Movies</a>
            </li>
            <li>
                <a href="#">TV</a>
            </li>
            <li>
                <a href="#">Games</a>
            </li>
            <li>
                <a href="#">Collectibles</a>
            </li>
            <li>
                <a href="#">Videos</a>
            </li>
            <li>
                <a href="#">Fans</a>
            </li>
            <li>
                <a href="#">News</a>
            </li>
            <li>
                <a href="#">Shop</a>
            </li> -->
          </ul>


        </nav>
      </div>
    </header>
  </template>
  
  <script> 

    export default {
      
        data() {


		    return {

			    menuList: [
                    {label:'Characters', link: '#' },
                    {label:'Comics', link: '#' },
                    {label:'Movies', link: '#' },
                    {label:'TV', link: '#' },
                    {label:'Games', link: '#' },
                    {label:'Collectibles', link: '#' },
                    {label:'Videos', link: '#' },
                    {label:'News', link: '#' },
                    {label:'Shop', link: '#' },
                ],
		    }
        },
    }
  </script>

  <style lang="scss" scoped>
@use '../style/partials/variables' as *;

  .logo{
  width: 70px;
}

.header{
  background-color: $white;
  margin-top: 30px;
}

.header-menu{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  margin-top: 10px;
}

.menu-list{
  display: flex;
  list-style: none;
  gap: 15px;
  text-transform: uppercase;
}

.header-list-items{
    position: relative;

    &:hover{
        color: $main-blue;
    }

    &:hover::after{
        content: '';
        display: block;
        width: 40px;
        padding: 2px;
        background-color: $main-blue;
        position: absolute;
        top: 60px;
        left: 50%;
        transform: translateX(-50%);
    }
}

  </style>