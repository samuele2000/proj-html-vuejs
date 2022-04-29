<template>
    <div class="bg_color py_5">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="rows">
                <div class="text">
                   <h6 class="title-2 c-fountain-blue">newsletter</h6>
                    <h2 class="title"><span class="text-custom">Know</span> First</h2>
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

    /*Inserire style componente*/
    // color
    .bg_color {
        background-color: $woodsmoke;
    }

    .bg-blue-lagoon {
        background-color: $blue-lagoon;
    }

    .containers {
        width: 70%;
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
    .mr-10{
        margin-right: 10px;
    }
    .p_30 {
        padding-top: 100px;
    }
    .p-relative {
        position: relative;
    }
    .opacity{
        opacity: 0;
    }
    .d-none{
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
    //fine utility
    
    .title {
        font-weight: bold;
        font-size: 2em;
        margin: 20px 0;
        color: #fff;
    }

    .title-2 {
        font-weight: bold;
        font-size: 0.8em;
        margin: 20px 0;
        text-transform: uppercase;
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
        align-items: baseline;
    }

    .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 20px;
        border-radius: 5px;
        border: none;
        margin-top: 5px;
    }
    .input{
        display: flex;
        flex-direction: column;
        flex-basis: 50%;
    }
    .text{
       margin-right: 50px;
    }
    .input-custom{
        background-color: $abbey-01;
        border: none;
        padding: 10px 10px;
        margin: 10px 0;
    }
</style>