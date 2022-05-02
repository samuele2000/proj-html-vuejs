<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <h6 class="c-fountain-blue">our business areas</h6>
            <h2>Excellence in <span class="text-custom">Services</span></h2>
            <div class="row">
                <div class="paragraph">
                    <p class="c-silver-sand">We are leaders in providing consultancy services with a set of cutting-edge
                        technologies and a team of experienced and renowed professional. these are some options that you
                        can hire</p>
                </div>

                <div>
                    <button type="button" class="button-empty">see
                        all</button>
                </div>

            </div>

            <div class="container">
                <div v-for="(element, index) in Services" :key="index" class="bg_color_2 box">
                    <div class="box-2">
                        <div>
                            <span class="c-blue-lagoon"><i :class="`${element.icona}`"></i></span>
                            <span class="c-blue-lagoon"><i :class="`${element.freccia}`" class="arrow"></i></span>
                        </div>
                        <h6>{{element.servizio}}</h6>
                        <p class="c-silver-sand pb-5">{{element.descrizione}}</p>
                    </div>


                </div>
            </div>
        </div>


    </div>
</template>

<script>
    export default {
        //Cambiare il nome con quello del componente creato
        name: 'ServicesComp',
        data() {
            return {
                Services: [{
                        servizio: 'Audit & Assurance',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-circle-nodes',
                        freccia: 'fa-solid fa-arrow-right-long'
                    },
                    {
                        servizio: 'Financial Advisory',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-briefcase',
                        freccia: 'fa-solid fa-arrow-right-long'
                    },
                    {
                        servizio: 'Analytics and M&A',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-chart-simple',
                        freccia: 'fa-solid fa-arrow-right-long'
                    },
                    {
                        servizio: 'Middle Marketing',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-plane-up',
                        freccia: 'fa-solid fa-arrow-right-long'
                    },
                    {
                        servizio: 'Legal Consulting',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-scale-balanced',
                        freccia: 'fa-solid fa-arrow-right-long'
                    },
                    {
                        servizio: 'Regulatory Risk',
                        descrizione: 'Lorem ipsum dolor sit amet,consectetur adipiscing elit.',
                        icona: 'fa-solid fa-inbox',
                        freccia: 'fa-solid fa-arrow-right-long'
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
    .bg_color {
        background-color: $woodsmoke;
    }

    .bg_color_2 {
        background-color: $abbey-01;
    }

    .c-silver-sand {
        color: $silver-sand;
    }

    .border-blue-lagoon {
        border: 1px solid $blue-lagoon;
    }

    .c-fountain-blue {
        color: $fountain-blue;
    }

    .c-blue-lagoon {
        color: $blue-lagoon;
    }

    .text-custom {
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    .py_5 {
        padding: 100px 0;
    }

    .button-empty {
        background-color: transparent;
        border: 1px solid $blue-lagoon;
        text-transform: uppercase;
        color: #fff;
        padding: 10px 20px;
        border-radius: 5px;
        margin-top: 20px;
    }

    // fine utility


    .containers {
        width: 80%;
        margin: 0 auto;

        h2 {
            padding-top: 20px;
            font-family: 'Poppins', sans-serif;
            font-size: 2.2em;
            color: #fff;
        }

        h6 {
            text-transform: uppercase;
            font-size: 0.8em;
        }

        .row {
            display: flex;
            justify-content: space-between;

            .paragraph {
                width: 70%;
                padding: 20px 0;
            }

        }
    }

    .container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;

        .box {
            width: calc((100% / 3) - 15px);
            color: #fff;
            margin-top: 20px;
            border-radius: 5px;
        }

        .box-2 {
            width: 75%;
            margin: 0 auto;
            padding: 30px 0;

            div {
                display: flex;
                justify-content: space-between;
                margin-bottom: 10px;

                span {
                    font-size: 2em;
                    padding-top: 10px;
                }
            }

            h6 {
                font-size: 1.1em;
                margin-bottom: 20px;
                margin-top: 20px;
            }
            p{
                padding-bottom: 30px;
            }
        }
    }
    // hover
    .box-2:hover{
        p{
            color: #fff;
        }
        span{
            color: #fff;
        }
        .arrow{
            background-color: $blue-lagoon;
            width: 40px;
            height: 40px;
            line-height: 40px;
            border-radius: 50%;
            text-align: center;

        }
    }
        .button-empty:hover {
        background-color: $fountain-blue;
        border-color: $fountain-blue;
        color: #fff;
    }
    
</style>