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
                <a :href="comics.link">
                    {{ comics.label }}
                </a>
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
                <a :href="shop.link">
                    {{ shop.label }}
                </a>
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
                <a :href="dc.link">
                    {{ dc.label }}
                </a>
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
                <a :href="sites.link">
                    {{ sites.label }}
                </a>
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

          <img class="position" src="../../public/dc-logo-bg.png" alt="">

        </div>

        
      </div>
    </main>
  </template>

<script>
  export default {
    
    data(){

        return{

            comicsList: [
                {label:'Characters', link: '#' },
                {label:'Comics', link: '#' },
                {label:'Movies', link: '#' },
                {label:'TV', link: '#' },
                {label:'Games', link: '#' },
                {label:'Videos', link: '#' },
                {label:'News', link: '#' },
            ],

            shopList: [

                {label:'Shop SC', link: '#' },
                {label:'Sho DC Collectibles', link: '#' },
            ],

            dcList: [
                {label:'Term of Use', link: '#' },
                {label:'Privacy Policy', link: '#' },
                {label:'Ad Choices', link: '#' },
                {label:'Advertising', link: '#' },
                {label:'Jobs', link: '#' },
                {label:'Subscription', link: '#' },
                {label:'Takent Workshops', link: '#' },
                {label:'CPSC Certificates', link: '#' },
                {label:'Ratings', link: '#' },
                {label:'Shop help', link: '#' },
                {label:'Contact us', link: '#' },
            ],

            siteList: [
                {label:'DC', link: '#' },
                {label:'MAD Magazine', link: '#' },
                {label:'DC Kids', link: '#' },
                {label:'DC Universe', link: '#' },
                {label:'DC Power Visa', link: '#' },
            ]
        }
    }
  }
</script>

<style lang="scss" scoped>


</style>