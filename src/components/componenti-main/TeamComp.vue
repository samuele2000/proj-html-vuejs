<template>
    <div class="py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="box">
                <div class="text-left">
                    <h6 class="c-fountain-blue">we like what we do</h6>
                    <h2><span class="text-custom">Team</span> of Experts</h2>
                    <p class="c-silver-sand">
                        Ethics and integrity are the bases on which our professionals build their careers. They are
                        fundamentals that become daily attidudes.
                    </p>
                    <!-- sezione con i 4 dipendenti -->
                    <div class="team">
                        <div v-for="(element, index) in Team" :key="index" class="card">
                            <img :src="element.numeroFoto" alt="">
                            <div>
                                <h5>{{element.nome}}</h5>
                                <h6 class="c-silver-sand">{{element.posizione}}</h6>
                                <div class="icon">
                                    <a href="#" class="bg_surfiegreen c-blue-lagoon circle "><i
                                            :class="`${element.iconafb}`"></i></a>
                                    <a href="#" class="bg_surfiegreen c-blue-lagoon circle"><i
                                            :class="`${element.iconatw}`"></i></a>
                                    <a href="#" class="bg_surfiegreen c-blue-lagoon circle"><i
                                            :class="`${element.iconain}`"></i></a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- parte del testo (president speech) -->
                <div class="bg_blue-lagoon speech">
                    <h4>President Speech</h4>
                    <div>
                        <p class="c-silver-sand">
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci fugiat quisquam in.
                        </p>
                        <p class="c-silver-sand">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione nostrum mollitia vel
                            accusamus
                            corrupti beatae laboriosam.
                        </p>
                        <p class="c-silver-sand">
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aut nobis rerum unde!
                        </p>
                    </div>
                    <div class="author">
                        <h6 class="c-silver-sand">T.Johnson</h6>
                        <span class="c-shark"><i class="fa-solid fa-quote-right"></i></span>
                    </div>

                </div>

            </div>


        </div>


    </div>
</template>

<script>
    export default {
        //Cambiare il nome con quello del componente creato
        name: 'TeamComp',
        data() {
            return {
                Team: [{
                        nome: 'David Cooper',
                        posizione: 'CTO & CO-FOUNDER',
                        iconafb: 'fa-brands fa-facebook-f',
                        iconatw: 'fa-brands fa-twitter',
                        iconain: 'fa-brands fa-linkedin-in',
                        numeroFoto: require('../../assets/img/team-1.jpg')
                    },
                    {
                        nome: 'Oliver Jones',
                        posizione: 'CHIEF PROCURAMENT ',
                        iconafb: 'fa-brands fa-facebook-f',
                        iconatw: 'fa-brands fa-twitter',
                        iconain: 'fa-brands fa-linkedin-in',
                        numeroFoto: require('../../assets/img/team-3.jpg')
                    },
                    {
                        nome: 'Emma Lopez',
                        posizione: 'CHIEF MARKETING',
                        iconafb: 'fa-brands fa-facebook-f',
                        iconatw: 'fa-brands fa-twitter',
                        iconain: 'fa-brands fa-linkedin-in',
                        numeroFoto: require('../../assets/img/team-2.jpg')
                    },
                    {
                        nome: 'T.Johnson',
                        posizione: 'CEO & PRESIDENT',
                        iconafb: 'fa-brands fa-facebook-f',
                        iconatw: 'fa-brands fa-twitter',
                        iconain: 'fa-brands fa-linkedin-in',
                        numeroFoto: require('../../assets/img/team-4.jpg')
                    },
                ]
            }
        }

    }
</script>

<style scoped lang="scss">
    @import '../../style/variabili.scss';

    /*Inserire style componente*/
    //  utility
    .py_5 {
        padding: 100px 0;
    }

    .c-fountain-blue {
        color: $fountain-blue;
    }


    .c-silver-sand {
        color: $silver-sand;
    }

    .c-shark {
        color: $shark;
    }

    .c-blue-lagoon {
        color: $blue-lagoon;
    }

    .bg_surfiegreen {
        background-color: $surfiegreen;
    }

    .bg_blue-lagoon {
        background-color: $blue-lagoon;
    }

    .bg_color_2 {
        background-color: $abbey-01;
    }

    .circle {
        width: 30px;
        height: 30px;
        border-radius: 50%;
        text-align: center;
        line-height: 30px;
    }

    .text-custom {
        color: $blue-lagoon;
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    // fine utility
    .containers {
        width: 80%;
        margin: 0 auto;

        .box {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .text-left {
                width: 60%;

                h2 {
                    padding-top: 20px;
                    font-family: 'Poppins', sans-serif;
                    font-size: 2.2em;
                }

                h6 {
                    text-transform: uppercase;
                    font-size: 0.8em;
                }

                p {
                    padding-top: 20px;
                    padding-bottom: 40px;
                }

                .team {
                    display: flex;
                    justify-content: space-between;
                    flex-wrap: wrap;

                    .card {
                        width: 50%;
                        display: flex;
                        margin-bottom: 40px;

                        img {
                            width: 30%;
                            border-radius: 5px;
                            margin-right: 20px;
                        }

                        div {
                            h5 {
                                font-size: 1.1em;
                                margin-bottom: 10px;
                            }

                            .icon {
                                display: flex;
                                margin-top: 20px;

                                a {
                                    margin-right: 5px;
                                }
                            }
                        }
                    }
                }
            }

            .speech {
                width: 30%;
                padding: 30px;
                border-radius: 5px;

                h4 {
                    color: #fff;
                    font-size: 1.5em;
                    margin-bottom: 30px;
                }

                p {
                    margin-bottom: 20px;
                }
                .author{
                   display: flex; 
                   justify-content: space-between;
                   font-size: 1.5em;
                }
                    
                
            }
        }
    }
</style>