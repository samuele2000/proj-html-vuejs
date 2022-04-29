<template>
    <div class="py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="d-flex justify-content-between">
                <div class="col-7">
                    <h6 class="text-uppercase c-fountain-blue">we like what we do</h6>
                    <h2 class="fs-1 fw-bold my-3"><span class="text-custom">Team</span> of Experts</h2>
                    <p class="c-silver-sand">
                        Ethics and integrity are the bases on which our professionals build their careers. They are
                        fundamentals that become daily attidudes.
                    </p>
                    <!-- sezione con i 4 dipendenti -->
                    <div class=" d-flex justify-content-between flex-wrap">
                        <div v-for="(element, index) in Team" :key="index" class=" mt-4 rounded col-6 d-flex mb-4">
                            <img :src="element.numeroFoto" alt="" class="w-25 rounded">
                            <div class="ms-4">
                                <h5>{{element.nome}}</h5>
                                <h6 class="c-silver-sand mb-3">{{element.posizione}}</h6>
                                <div class="d-flex">
                                    <a href="#" class="bg_surfiegreen c-blue-lagoon circle "><i
                                            :class="`${element.iconafb}`"></i></a>
                                    <a href="#" class="bg_surfiegreen mx-2 c-blue-lagoon circle"><i
                                            :class="`${element.iconatw}`"></i></a>
                                    <a href="#" class="bg_surfiegreen c-blue-lagoon circle"><i
                                            :class="`${element.iconain}`"></i></a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- parte del testo (president speech) -->
                <div class="col-3 bg_blue-lagoon py-4 px-4 rounded">
                    <h4 class="mb-4 text-light fw-bold">President Speech</h4>
                    <p class="c-silver-sand"> 
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci fugiat quisquam in. 
                    </p>
                    <p class="c-silver-sand">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione nostrum mollitia vel accusamus corrupti beatae laboriosam.
                    </p>
                    <p class="c-silver-sand">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aut nobis rerum unde!
                    </p>
                    <div class="d-flex justify-content-between">
                        <h6 class="c-silver-sand">T.Johnson</h6>
                        <span class="fs-4 c-shark"><i class="fa-solid fa-quote-right"></i></span>  
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
    .bg_surfiegreen {
        background-color: $surfiegreen;
    }

    .bg_blue-lagoon {
        background-color: $blue-lagoon;
    }

    .bg_color_2 {
        background-color: $abbey-01;
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
    .c-shark{
        color: $shark;
    }


    .text-custom {
        color: $blue-lagoon;
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    .py_5 {
        padding: 100px 0;
    }

    .c-fountain-blue {
        color: $fountain-blue;
    }

    .circle {
        width: 30px;
        height: 30px;
        border-radius: 50%;
        text-align: center;
        line-height: 30px;
    }
</style>