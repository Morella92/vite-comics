<template>
    <main>
      <div class="container">

        <div class="main-content">
          <button class="button-cards position-button">current series</button>
        </div>

        <div class="container">
            <div class="row-cards">
                <CardMain v-for="(element, index) in cardsList" :key="index" 
                :card="element"/>
            </div>

            <div class="row-cards">
                <button class="button-cards">
                    load more
                </button>
            </div>
        </div>

        <div class="row-brands">

          <ul class="list-brand">
            <li>
                <a class="list-brands-items" href="#">
                    <img class="list-brands-images" src="../../public/buy-comics-digital-comics.png" alt="">
                    <h3 class="list-brands-description">digital comics</h3>
                </a>  
            </li>
            <li>
                <a class="list-brands-items" href="#">
                    <img class="list-brands-images" src="../../public/buy-comics-merchandise.png" alt="">
                    <h3 class="list-brands-description">mc merchandise</h3>
                </a>
            </li>
            <li>
                <a class="list-brands-items" href="#">
                    <img class="list-brands-images" src="../../public/buy-comics-subscriptions.png" alt="">
                    <h3 class="list-brands-description">subscription</h3>
                </a>
            </li>
            <li>
                <a class="list-brands-items" href="#">
                    <img class="list-brands-images" src="../../public/buy-comics-shop-locator.png" alt="">
                    <h3 class="list-brands-description">comic shop locator</h3>
                </a>
            </li>
            <li>
                <a class="list-brands-items" href="#">
                    <img class="list-brands-images" src="../../public/buy-dc-power-visa.svg" alt="">
                    <h3 class="list-brands-description">dc power visa </h3>
                </a>
            </li>
          </ul>

        </div>

        <div class="row-hero"> 

          <ul class="list-hero">
            <li class="list-title"> 
                <h4>dc comics</h4>
            </li>
            <li class="list-hero-items" v-for="(comics, index) in comicsList" :key="index">
                <a :href="comics.link">
                    {{ comics.label }}
                </a>
            </li>

            <li class="list-title">
                <h4>shop</h4>
            </li>
            <li class="list-hero-items" v-for="(shop, index) in shopList" :key="index">
                <a :href="shop.link">
                    {{ shop.label }}
                </a>
            </li>
          </ul>

          <ul class="list-hero">
            <li class="list-title">
                <h4>DC</h4>
            </li>
            <li class="list-hero-items" v-for="(dc, index) in dcList" :key="index">
                <a :href="dc.link">
                    {{ dc.label }}
                </a>
            </li>
          </ul>

          <ul class="list-hero">
            <li class="list-title"> 
                <h4>sites</h4>
            </li>
            <li class="list-hero-items" v-for="(sites, index) in siteList" :key="index">
                <a :href="sites.link">
                    {{ sites.label }}
                </a>
            </li>
          </ul>

          <img class="position" src="../../public/dc-logo-bg.png" alt="">

        </div>
     
      </div>
    </main>
  </template>

<script>
import CardMain from './CardMain.vue'

  export default {
    components:{
        CardMain
    },

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
            ],

            cardsList: [
                {
                    "thumb": "../../public/image-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-2.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-3.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "../../public/image-4.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-5.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-6.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-7.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-8.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-9.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-10.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {   "thumb": "../../public/image-11.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "../../public/image-12.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
.main-content{
    background-image: url('../../public/jumbotron.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    min-height: 350px;
    position: relative;
}

.position-button{
    position: absolute;
    bottom: -40px;
    left: 20px;
}
.row-cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.button-cards{
    color: $white;
    background-color: $main-blue;
    text-transform: uppercase;
    font-weight: 600;
    padding: 15px;
    margin-bottom: 20px;
    border: none;
}
.row-brands{
  color: $white;
  background-color: $main-blue ;
  padding: 20px;
}
.list-brand{
  display: flex;
  list-style: none;
  gap: 30px;
  justify-content: center;
  align-items: center;
  z-index: 2;
}

.list-brands-items{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;

  &:hover{
    color: rgba($color: #a38f8f, $alpha: 1.0);
  }
}
.list-brands-images{
  width: 40px;

  &:hover{
    color: rgba($color: #a38f8f, $alpha: 1.0);
  }
}

.list-brands-description{
  text-transform: uppercase;
  font-size: 15px;
}

.row-hero{
  background-image: url('../public/footer-bg.jpg');
  display: flex;
  position: relative;
}

.position{
  width: 400px;
  position: absolute;
  right: 200px;
  bottom: 0;
  top: -50px;
}
.list-hero{
  list-style: none;
  padding-left: 20px;
  color: $white;
  padding-bottom: 20px;
}

.list-title{
  text-transform: uppercase;
  font-size: 20px;
  padding-top: 20px;
}

.list-hero-items{

    &:hover{
        color: $main-blue;
    }
}
</style>