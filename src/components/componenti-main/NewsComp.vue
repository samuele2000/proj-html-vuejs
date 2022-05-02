<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="text">
                <h6 class="c-fountain-blue">our editorial content</h6>
                <h2>Latest <span class="text-custom">News</span></h2>
            </div>
            <div class="rows">
                <div>
                    <p class="c-silver-sand">
                        Every week we publish content about what is best in the business world.
                    </p>
                </div>
                <!-- bottone -->
                <div>
                    <button type="button" class="button-all bg-blue-lagoon">see all</button>

                </div>
            </div>


            <div class="rows">

                <div v-for="(element, index) in News" :key="index" class="box img p-relative"
                    :style="{ backgroundImage:`url(${element.img})`}">
                    <div class="overlay"></div>
                    <div class="blur"></div>
                    <div class="box-internal">
                        <div class="top">
                            <div>
                                <span class="mr-10"><i :class="`${element.iconaUser}`"></i></span>
                                <span class="">{{element.nome}}</span>
                            </div>
                            <div>
                                <span class="mr-10"><i :class="`${element.iconaDay}`"></i></span>
                                <span class="">{{element.data}}</span>
                            </div>
                        </div>
                        <div class="bottom">
                            <h6 class="fs_2">{{element.notizia}}</h6>
                            <p class="c-silver-sand d-none">{{element.descrizione}}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>


    </div>
</template>

<script>
    export default {
        //Cambiare il nome con quello del componente creato
        name: 'NewsComp',
        data() {
            return {
                News: [{
                        nome: 'Andrea Miller',
                        data: '2 Days Ago',
                        notizia: 'Increasing creativity is possible for everyone',
                        descrizione: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
                        iconaUser: 'fa-regular fa-user',
                        iconaDay: 'fa-regular fa-clock',
                        img: require('../../assets/img/news-1.jpg')
                    },
                    {
                        nome: 'Andrea Miller',
                        data: '1 Days Ago',
                        notizia: 'Because amrket research is part of the business plan',
                        descrizione: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
                        iconaUser: 'fa-regular fa-user',
                        iconaDay: 'fa-regular fa-clock',
                        img: require('../../assets/img/news-2.jpg')
                    },
                    {
                        nome: 'Andrea Miller',
                        data: '5 Days Ago',
                        notizia: 'Working froom home is now a trend',
                        descrizione: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
                        iconaUser: 'fa-regular fa-user',
                        iconaDay: 'fa-regular fa-clock',
                        img: require('../../assets/img/news-3.jpg')
                    },
                ]
            }
        }

    }
</script>

<style scoped lang="scss">
    @import '../../style/variabili.scss';

    /*Inserire style componente*/
    // color
    .bg_color {
        background-color: $gray-nurse;
    }

    .bg-blue-lagoon {
        background-color: $blue-lagoon;
    }

    .containers {
        width: 80%;
        margin: 0 auto;
    }

    .c-blue-lagoon {
        color: $blue-lagoon;
    }

    .c-silver-sand {
        color: $silver-sand;
    }

    .c-fountain-blue {
        color: $fountain-blue;
    }

    // utility
    .fs_2 {
        font-size: 1.6em;
    }

    .py_5 {
        padding: 100px 0;
    }

    .mr-10 {
        margin-right: 10px;
    }

    .p_30 {
        padding-top: 100px;
    }

    .p-relative {
        position: relative;
    }

    .overlay {
        background-color: rgba(0, 0, 0, 0.5);
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        border-radius: 10px;
    }

    //fine utility
    .text {
        margin-right: 50px;

        h2 {
            padding-top: 20px;
            font-family: 'Poppins', sans-serif;
            font-size: 2.2em;
            margin-bottom: 20px;
        }

        h6 {
            text-transform: uppercase;
            font-size: 0.8em;
        }

        p {
            padding-top: 20px;
            padding-bottom: 40px;
        }
    }

    .title {
        font-weight: bold;
        font-size: 2em;
        margin: 20px 0;
    }

    .title-2 {
        font-weight: bold;
        font-size: 0.8em;
        margin: 20px 0;
        text-transform: uppercase;
    }

    .text-custom {
        color: $blue-lagoon;
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    .rows {
        display: flex;
        justify-content: space-between;
        align-content: center;
    }

    .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 15px;
        border-radius: 5px;
        border: none;
    }

    .button-all:hover {
        background-color: $fountain-blue;
    }

    .box-internal {
        width: 80%;
        margin: 0 auto;
    }

    .box {
        width: calc((100% / 3) - 15px);
        height: 350px;
        border-radius: 10px;
        margin-top: 30px;
    }

    .box:hover {
        .box-internal {
            z-index: 2;
            .top {
                opacity: 1;
            }

            .bottom {
                p {
                    display: block;
                }
            }
        }



    }

    .img {
        background-size: cover;
        background-position: center;
    }

    .top {
        display: absolute;
        display: flex;
        justify-content: space-between;
        margin-top: 30px;
        color: white;
        opacity: 0;

        div {
            z-index: 2;
        }
    }

    .bottom {
        text-align: center;
        color: white;
        position: absolute;
        bottom: 40px;
        right: 10%;
        left: 10%;

        p {
            display: none;
            margin-top: 15px;
        }
    }
</style>