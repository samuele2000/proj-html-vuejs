<template>
    <div class="py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="rows">
                <div class="input">
                    <div class="text">
                        <h6 class="c-fountain-blue">send a message</h6>
                        <h2>Get in <span class="text-custom c-blue-lagoon">Touch</span></h2>
                        <p class="c-silver-sand">
                            We will responde to your message as soon as possible.
                        </p>
                    </div>
                    <div>
                        <input class="input-custom mr_10" type="text" placeholder="Name">
                        <input class="input-custom" type="email" placeholder="Email">
                    </div>
                    <div>
                        <input class="input-custom mr_10" type="numeber" placeholder="Phone">
                        <input class="input-custom" type="text" placeholder="More Info">
                    </div>

                    <input class="input-custom-message" type="message" placeholder="Message">


                    <div>
                        <button type="button" class="button-all bg-blue-lagoon">send</button>
                    </div>
                </div>
                <!-- info -->
                <div>
                    <div class="box-internal">
                        <h6>Example Inc.</h6>
                        <p class="c-silver-sand">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                        <p class="c-silver-sand">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <div class="info">
                            <span class="c-blue-lagoon"><i class="fa-solid fa-phone circle bg_surfiegreen mr_10"></i>+1
                                (305) 1234-5678</span>
                            <span class="c-blue-lagoon"><i
                                    class="fa-solid fa-envelope my_40 circle bg_surfiegreen mr_10"></i>hello@example.com</span>
                            <span class="c-blue-lagoon"><i
                                    class="fa-solid fa-location-dot circle bg_surfiegreen mr_10"></i>Main Avenue,
                                987</span>
                            <div>
                                <button type="button" class="button-empty">view map</button>
                            </div>

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
        name: 'MessageComp',

    }
</script>

<style scoped lang="scss">
    @import '../../style/variabili.scss';
    @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
    /*Inserire style componente*/
    // color
    .bg-blue-lagoon {
        background-color: $blue-lagoon;
    }

    .bg_surfiegreen {
        background-color: $surfiegreen;
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

    .mr_10 {
        margin-right: 20px !important;
    }

    .my_40 {
        margin: 40px 0;
    }
    
    .circle {
        width: 35px;
        height: 35px;
        border-radius: 50%;
        text-align: center;
        line-height: 35px;
    }

    //fine utility
    .containers {
        width: 80%;
        margin: 0 auto;
    }
    .text {
        margin-right: 50px;

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
    }
    .text-custom {
        background-color: $surfiegreen;
        padding: 3px 6px;
        border-radius: 5px;
    }

    .rows {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
    }

    .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 20px;
        border-radius: 5px;
        border: none;
        margin-top: 20px;
    }

    .button-all:hover {
        background-color: $fountain-blue;
    }

    .button-empty {
        background-color: transparent;
        border: 1px solid $blue-lagoon;
        text-transform: uppercase;
        color: $blue-lagoon;
        padding: 10px 20px;
        border-radius: 5px;
        margin-top: 20px;
    }

    .button-empty:hover {
        background-color: $fountain-blue;
        border-color: $fountain-blue;
        color: #fff;
    }

    .input {
        display: flex;
        flex-direction: column;
        flex-basis: 60%;
    }



    .input-custom {
        background-color: $abbey-01;
        border: none;
        padding: 10px 10px;
        margin-top: 10px;
        margin-bottom: 10px;
        border-radius: 5px;
        width: calc((100% / 2) - 10px);
    }

    .input-custom-message {
        background-color: $abbey-01;
        border: none;
        padding: 10px 10px;
        margin: 10px 0;
        padding-bottom: 150px;
        border-radius: 5px;
    }

    .info {
        display: flex;
        flex-direction: column;
        margin-top: 40px;
    }

    .box-internal {
        width: 80%;
        margin: 0 auto;

        h6 {
            font-weight: bold;
            font-size: 1.3em;
        }
        p{
            margin: 20px 0;
        }
    }
</style>