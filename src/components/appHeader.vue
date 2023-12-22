<script>
export default {
    data(){
        return{
            options : [
                "CHARACTERS",
                "COMICS",
                "MOVIE",
                "TV",
                "GAMES",
                "COLLECTIBLES",
                "VIDEOS",
                "FANS",
                "FANS",
                "NEWS",
                "SHOP"
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="logo">
            <img src="../../vue-dc-comics-1/img/dc-logo.png" alt="">
        </div>
        <div class="header-menu">
            <div v-for="option in options">
                <span>{{option}}</span>
            </div>
            
        </div>
    </header>
</template>

<style lang="scss" scoped>

    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }


    header{
        min-height: 100px;
        width: 100vw;
        display: flex;
        justify-content: space-around;
        border-bottom: 1px solid black;

        div{
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .logo{
            width: 100px;
            height: 100%;
            padding: 10px;

            img{
                width: 100%;
                height: 100%;
            }
        }

        .header-menu{
            display: flex;

            div{
                height: 100%;
                display: flex;
                margin: 0 5px;
                align-items: center;
                font-weight: bold;
                font-size: 0.8em;
            }
        }
    }
</style>