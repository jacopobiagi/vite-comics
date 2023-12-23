<script>
    export default{
        data(){
            return {
                objShop: [
                    {
                        img: '../../vue-dc-comics-1/img/buy-comics-digital-comics.png',
                        desc: 'DIGITAL COMICS'
                    },
                    {
                        img: '../../vue-dc-comics-1/img/buy-comics-merchandise.png',
                        desc: 'DC MERCHANDISE'
                    },
                    {
                        img: '../../vue-dc-comics-1/img/buy-comics-subscriptions.png',
                        desc: 'SUBSCRIPTION'
                    },
                    {
                        img: '../../vue-dc-comics-1/img/buy-dc-power-visa.svg',
                        desc: 'COMIC SHOP LOCATOR'
                    },
                    {
                        img: '../../vue-dc-comics-1/img/buy-comics-digital-comics.png',
                        desc: 'DC POWER VISA'
                    },
                ]
            }
        }
    }
</script>

<template>
    <main>
        <div class="content">
            <h2>
                Content goes Here
            </h2>
        </div>
        <div class="shop">
            <div v-for="obj in objShop">
                <div>
                    <img :src="obj.img" alt="d-c">
                </div>
                <h3>{{ obj.desc }}</h3>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    main{
        width: 100vw;
        .content{
            width: 100%;
            height: 100px;
            display: flex;
            align-items: center;
            padding: 0 10%;
            background-color: black;

            h2{
                color: white;
            }
        }

        .shop{
            padding: 0 5%;
            display: flex;
            background-color: rgb(2, 130, 249);
            height: 120px;

            div{
                width: calc(100% / 5);
                display: flex;
                justify-content: center;
                align-items: center;

                div{
                    width: 40px;
                    margin-right: 5px;

                    img{
                        width: 100%;
                    }
                }
                h3{
                    color: white;
                    font-size: 0.7em;
                    font-weight: 400;
                }
            }
        }
    }
</style>