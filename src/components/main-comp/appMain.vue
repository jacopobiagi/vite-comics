<script>
import cards from '../../models/dc-comics.json';
import card from './sub-comp/cards.vue';

export default {
    components : {
        card
    },
    data() {
        return {
            cards
        }
    }
}
</script>

<template>
    <div class="window"></div>

    <div class="content">
        <card v-for="element in cards"
        :img = "element.thumb"
        :price = "element.price"
        :series = "element.series"
        :type = "element.type" />
    </div>
</template>

<style lang="scss" scoped>
    .window{
        height: 300px;
        background-image: url('../../../vue-dc-comics-1/img/jumbotron.jpg');
        background-size: cover;
        img{
            width: 100%;
            height: 100%;
        }
    }
    .content {
        //width: 100vw;
        min-height: 100px;
        display: flex;
        flex-wrap: wrap;
        align-items: flex-start;
        padding: 0 10%;
        background-color: black;

        h2 {
            color: white;
        }
    }
</style>