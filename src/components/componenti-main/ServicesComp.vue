<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <h6 class="text-uppercase">our business areas</h6>
            <h2 class="fs-1 fw-bold py-3 text-light">Excellence in <span class="text-custom">Services</span></h2>
            <div class="d-flex justify-content-between">
                <div class="col-8">
                    <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowed professional. these are some options that you can hire</p>
                </div>

                <div>
                    <button type="button" class="btn text-uppercase text-light fw-bold border-blue-lagoon px-3">see all</button>
                </div>

            </div>

            <div class=" d-flex justify-content-between">
                <div v-for="(element, index) in numberUtility" :key="index" class="text-light d-flex flex-column mt-5">
                    <span class="c-fountain-blue fw-bold fs-3">{{element.numero}}</span>
                    <span class="fw-bold fs-5">{{element.nome}}</span>
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

    .containers {
        width: 80%;
        margin: 0 auto;
    }

    h6 {
        color: $blue-lagoon;
    }

    p {
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
</style>