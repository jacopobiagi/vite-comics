<script>
export default{
    data(){
        return{
            social:[
                '../../vue-dc-comics-1/img/footer-facebook.png',
                '../../vue-dc-comics-1/img/footer-twitter.png',
                '../../vue-dc-comics-1/img/footer-youtube.png',
                '../../vue-dc-comics-1/img/footer-pinterest.png',
                '../../vue-dc-comics-1/img/footer-periscope.png'
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="dc-block">
            <div class="dc-lists">
                <div>
                    <h3>DCCOMICS</h3>
                    <span>Characters</span>
                    <span>comics</span>
                    <span>movies</span>
                    <span>TV</span>
                    <span>Games</span>
                    <span>Videos</span>
                    <span>News</span>

                    <h3>SHOP</h3>
                    <span>Shop Dc</span>
                    <span>Shop DC collectibles</span>
                </div>
                <div>
                    <h3>DC</h3>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                    <span>therms of use</span>
                </div>
                <div>
                    <h3>SITES</h3>
                    <span>DC</span>
                    <span>Mad magazine</span>
                    <span>DC kids</span>
                    <span>DC universe</span>
                    <span>DC power visa</span>
                </div>
            </div>
            <div class="big-logo">
                <img src="../../vue-dc-comics-1/img/dc-logo-bg.png" alt="big-logo">
            </div>
        </div>
        <div class="sign-up">
            <div class="sign-block">
                <h3>SIGN-UP NOW!</h3>
            </div>

            <div class="social-network">
                <div class="follow">
                    <h3>follow us</h3>
                </div>
                <div v-for="net in social">
                    <img :src="net" alt="social">
                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>
    footer{
        height: calc(100vh - 320px);

        .dc-block,.sign-up{
            padding: 0 8%;
        }
        .dc-block{
            height: 75%;
            background-image: url('../../vue-dc-comics-1/img/footer-bg.jpg');
            display: flex;
            justify-content: space-between;
            align-items: center;

            .dc-lists{
                display: flex;

                div{
                    display: flex;
                    flex-direction: column;
                    margin: 0 10px;
                    color: white;

                    h3{
                        font-size: 0.9em;
                        margin: 5px 0;
                    }
                    span{
                        font-size: 0.77em;
                        color: rgb(128, 129, 130);
                    }
                }
            }

            .big-logo{
                height: 100%;
                display: flex;
                align-items: center;

                img{
                    height: 115%;
                }
            }
        }

        .sign-up{
            background-color: rgb(48, 48, 48);
            height: 25%;
            position: relative;
            z-index: 2;
            display: flex;
            align-items: center;
            justify-content: space-between;

            .sign-block{
                color: white;
                border: 2px solid rgb(2, 130, 249);
                height: 50px;
                padding: 10px;
            }

            .social-network{
                display: flex;

                *{
                    margin: 0 3px;
                }
                h3{
                    color: rgb(2, 130, 249);
                }
            }
        }
    }
</style>