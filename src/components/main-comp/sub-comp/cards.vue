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

    <div class="content-series">
        <div class="series">
            <img :src="img" alt="img" class="">
        </div>
        <span>{{ series }}</span>
    </div>
    

</template>

<style lang="scss" scoped>
    .content-series{
        width: calc(100% / 6);
        padding: 20px;

        .series{
            width: 100%;
            height: 130px;
            img{
                width: 100%;
                height: 100%;
            }
        }
        span{
            color: white;
            font-size: 0.9em;
        }
    }
    
</style>