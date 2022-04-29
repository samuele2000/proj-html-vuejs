<template>
    <div class="py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="rows">
                <div class="input">
                    <div class="text">
                        <h6 class="title-2 c-fountain-blue">send a message</h6>
                        <h2 class="title">Get in <span class="text-custom c-blue-lagoon">Touch</span></h2>
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

    /*Inserire style componente*/
    // color
    .bg-blue-lagoon {
        background-color: $blue-lagoon;
    }

    .bg_surfiegreen {
        background-color: $surfiegreen;
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

    .mr_10 {
        margin-right: 20px !important;
    }

    .my_40 {
        margin: 40px 0;
    }

    .p_30 {
        padding-top: 100px;
    }

    .p-relative {
        position: relative;
    }

    .opacity {
        opacity: 0;
    }

    .d-none {
        display: none;
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

    .circle {
        width: 35px;
        height: 35px;
        border-radius: 50%;
        text-align: center;
        line-height: 35px;
    }

    //fine utility

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
        padding: 5px 20px;
        border-radius: 5px;
        border: none;
        margin-top: 20px;
    }

    .button-empty {
        background-color: transparent;
        border: 1px solid $blue-lagoon;
        text-transform: uppercase;
        color: $blue-lagoon;
        padding: 5px 20px;
        border-radius: 5px;
        margin-top: 20px;
    }

    .input {
        display: flex;
        flex-direction: column;
        flex-basis: 60%;
    }

    .text {
        margin-right: 50px;
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
    .box-internal{
        width: 80%;
        margin: 0 auto;
        h6{
            font-weight: bold;
            font-size: 1.3em;
        }
    }
</style>