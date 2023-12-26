<script>
export default{
    props: {
        img: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>

<template>
    <div class="series">
        <img :src="img" alt="img" class="">
    </div>

</template>

<style lang="scss" scoped>
    .series{
        width: 110px;
        height: 90px;
        img{
            width: 100%;
            height: 100%;
        }
    }
</style>