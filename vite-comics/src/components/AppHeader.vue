<template>
    <header class="header">
      <div class="container">

        <nav class="header-menu">
            <img class="logo" src="../../public/dc-logo.png" alt="">

          <ul class="menu-list">

            <li v-for="(item, index) in menuList" :key="index">
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

  <style lang="scss">


  </style>