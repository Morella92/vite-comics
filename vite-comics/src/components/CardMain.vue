<template>
    <div class="col-cards" v-for="(card, index) in cardsList" :key="index">
        <img class="img-cards" :src="card.thumb" alt="">
        <p class="cards-p"> {{ card.series }}</p>
    </div>
</template>

<script>
    export default {

        props: {
            card: {
                thumb: String,
                series:String
            }
        }
    }
</script>