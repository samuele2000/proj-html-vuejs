<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <h6 class="text-uppercase c-fountain-blue">our business areas</h6>
            <h2 class="fs-1 fw-bold py-3 text-light">Excellence in <span class="text-custom">Services</span></h2>
            <div class="d-flex justify-content-between">
                <div class="col-8">
                    <p class="c-silver-sand">We are leaders in providing consultancy services with  a set of cutting-edge
                        technologies and a team of experienced and renowed professional. these are some options that you
                        can hire</p>
                </div>

                <div>
                    <button type="button" class="btn text-uppercase text-light fw-bold border-blue-lagoon px-3">see
                        all</button>
                </div>

            </div>

            <div class=" d-flex justify-content-between flex-wrap">
                <div v-for="(element, index) in Services" :key="index" class="text-light bg_color_2 box mt-4 rounded">
                    <div class="box-2">
                        <div class="mb-3 d-flex justify-content-between pt-5">
                            <span class="c-blue-lagoon fs-2"><i :class="`${element.icona}`"></i></span>
                            <span class="c-blue-lagoon fs-4"><i :class="`${element.freccia}`"></i></span>
                        </div>
                        <h6 class="text-light fw-bold fs-5">{{element.servizio}}</h6>
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
    .bg_color {
        background-color: $woodsmoke;
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

    .text-custom {
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

    .border-blue-lagoon {
        border: 1px solid $blue-lagoon;
    }

    .box-2 {
        width: 75%;
        margin: 0 auto;
    }
    .box{
        width: calc((100% / 3) - 15px);
    }
</style>