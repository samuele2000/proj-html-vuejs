<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="rows">
                <div class="text">
                    <h6 class="c-fountain-blue">newsletter</h6>
                    <h2><span class="text-custom">Know</span> First</h2>
                    <p class="c-silver-sand">
                        Follow closely and receive content about our company and the news of the current market.
                    </p>
                </div>

                <!-- input -->
                <div class="input">
                    <input class="input-custom" type="text" placeholder="Name">
                    <input class="input-custom" type="email" placeholder="Email">
                    <div>
                        <button type="button" class="button-all bg-blue-lagoon">subscribe</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        //Cambiare il nome con quello del componente creato
        name: 'NewsletterComp',

    }
</script>

<style scoped lang="scss">
    @import '../../style/variabili.scss';
    @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

    /*Inserire style componente*/
    // color
    .bg_color {
        background-color: $woodsmoke;
    }

    .bg-blue-lagoon {
        background-color: $blue-lagoon;
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

    //fine utility
    .containers {
        width: 70%;
        margin: 0 auto;
    }
    .text {
        margin-right: 50px;

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

        p {
            padding-top: 20px;
            padding-bottom: 40px;
        }
    }


    .text-custom {
        color: #fff;
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    .rows {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 20px;
        border-radius: 5px;
        border: none;
        margin-top: 5px;
    }
    .button-all:hover {
        background-color: $fountain-blue;
    }

    .input {
        display: flex;
        flex-direction: column;
        flex-basis: 50%;
    }

    .input-custom {
        background-color: $abbey-01;
        border: none;
        padding: 10px 10px;
        margin: 10px 0;
    }
</style>