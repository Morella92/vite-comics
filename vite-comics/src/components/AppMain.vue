<template>
    <main>
      <div class="container">

        <div>
          <h3 class="content-title"> --Content goes here--</h3>
        </div>

        <div class="row-brands">

          <ul class="list-brand">
            <li>
                <a class="list-items" href="#">
                    <img class="list-images" src="../../public/buy-comics-digital-comics.png" alt="">
                    <h3 class="list-items-description">digital comics</h3>
                </a>  
            </li>
            <li>
                <a class="list-items" href="#">
                    <img class="list-images" src="../../public/buy-comics-merchandise.png" alt="">
                    <h3 class="list-items-description">mc merchandise</h3>
                </a>
            </li>
            <li>
                <a class="list-items" href="#">
                    <img class="list-images" src="../../public/buy-comics-subscriptions.png" alt="">
                    <h3 class="list-items-description">subscription</h3>
                </a>
            </li>
            <li>
                <a class="list-items" href="#">
                    <img class="list-images" src="../../public/buy-comics-shop-locator.png" alt="">
                    <h3 class="list-items-description">comic shop locator</h3>
                </a>
            </li>
            <li>
                <a class="list-items" href="#">
                    <img class="list-images" src="../../public/buy-dc-power-visa.svg" alt="">
                    <h3 class="list-items-description">dc power visa </h3>
                </a>
            </li>
          </ul>

        </div>


        <div class="row-hero"> 

          <ul class="list-hero">
            <li class="list-title"> 
                <h4>dc comics</h4>
            </li>
            <li v-for="(comics, index) in comicsList" :key="index">
                {{ comics }}
            </li>
            <!-- <li>
                <a href="#">
                    Comics
                </a>
            </li>
            <li>
                <a href="#">
                    Movies
                </a>
            </li>
            <li>
                <a href="#">
                    TV
                </a>
            </li>
            <li>
                <a href="#">
                    Games
                </a>
            </li>
            <li>
                <a href="#">
                    Videos
                </a>
            </li>
            <li>
                <a href="#">
                    News
                </a>
            </li> -->

            <li class="list-title">
                <h4>shop</h4>
            </li>
            <li v-for="(shop, index) in shopList" :key="index">
                {{ shop }}
            </li>
            <!-- <li>
                <a href="#">
                    Shop DC
                </a>
            </li>
            <li>
                <a href="#">
                    Shop DC collectibles
                </a>
            </li> -->
          </ul>

          <ul class="list-hero">
            <li class="list-title">
                <h4>DC</h4>
            </li>
            <li v-for="(dc, index) in dcList" :key="index">
                {{ dc }}
            </li>
            <!-- <li>
                <a href="#">
                    Term of Use
                </a>    
            </li>
            <li>
                <a href="#">
                    Privacy policy
                </a>    
            </li>
            <li>
                <a href="#">
                    Ad Choices
                </a>    
            </li>
            <li>
                <a href="#">
                    Advertising
                </a>    
            </li>
            <li>
                <a href="#">
                    Jobs
                </a>    
            </li>
            <li>
                <a href="#">
                    Subscriptions
                </a>    
            </li>
            <li>
                <a href="#">
                    Talent Workshops
                </a>    
            </li>
            <li>
                <a href="#">
                    CPSC Certificates
                </a>    
            </li>
            <li>
                <a href="#">
                    Ratings
                </a>    
            </li>
            <li>
                <a href="#">
                    Shop Help
                </a>    
            </li>
            <li>
                <a href="#">
                    Contact Us
                </a>    
            </li> -->
          </ul>

          <ul class="list-hero">
            <li class="list-title"> 
                <h4>sites</h4>
            </li>
            <li v-for="(sites, index) in siteList" :key="index">
                {{ sites }}
            </li>
            <!-- <li>
                <a href="#">
                    DC
                </a>
            </li>
            <li>
                <a href="#">
                    MAD Magazine
                </a>
            </li>
            <li>
                <a href="#">
                    DC Kids
                </a>
            </li>
            <li>
                <a href="#">
                    DC Universe
                </a>
            </li>
            <li>
                <a href="#">
                    DC Power Visa
                </a>
            </li> -->
          </ul>

        </div>

      </div>
    </main>
  </template>

<script>
  export default {
    
    data(){

        return{

            comicsList: [

                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],

            shopList: [

                'Shop DC',
                'Shop DC collectibles'
            ],

            dcList: [
                'Term of Use',
                'Privacy policy',
                'Ad Chioces',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],

            siteList: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ]
        }
    }
  }
</script>

<style lang="scss" scoped>


</style>