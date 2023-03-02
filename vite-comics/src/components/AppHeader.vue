<template>
  <header class="header">
    <div class="container">

      <nav class="header-menu">
        <img class="logo" src="../../public/dc-logo.png" alt="">

        <ul class="menu-list">

          <HeaderNav v-for="(item, index) in menuList" :key="index"
            :menu="item">
          </HeaderNav>
        </ul>
      </nav>
    </div>
  </header>
</template>
  
<script> 
import HeaderNav from './HeaderNav.vue';

  export default {
      components:{
        HeaderNav
      },

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

</style>