<template>
    <div class="col-cards">
        <img class="img-cards" :src="card.thumb" alt="">
        <p class="cards-p"> {{ card.series }}</p>
    </div>
</template>

<script>
    export default {

        props: {

            card: {
                type: Object,
                required: true
            }
        }
    }
</script>

<style lang="scss" scoped>
.col-cards{
    flex-basis: calc(100% / 6);
    padding-left: 30px;
    padding-top: 20px;
}

.img-cards{
    width: 100px;
    display: block;
    aspect-ratio: 1/1;
}

.cards-p{
    color: white;
    text-transform: uppercase;
    padding: 20px 0;
    font-size: 13px;
}
</style>