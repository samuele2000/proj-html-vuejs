<template>
    <div class="py_5 bg_image">
        <!--inserire contenuto componente-->
        <div class="containers">
            <div class="rows">
                <!-- info -->
                <div>
                    <div class="box-internal">
                        <div class="logo">
                            <h2><span class="nex-custom">nex</span><span class="gen-custom">gen</span></h2>
                        </div>
                        <p class="c-silver-sand">A functionalHTML Template for Corporate & Business</p>
                        <div class="info">
                            <span class="c-silver-sand"><i class="fa-solid fa-phone mr_10"></i>+1
                                (305) 1234-5678</span>
                            <span class="c-silver-sand"><i
                                    class="fa-solid fa-envelope my_40 mr_10"></i>hello@example.com</span>
                            <span class="c-silver-sand"><i class="fa-solid fa-location-dot mr_10"></i>Main Avenue,
                                987</span>
                            <div>
                                <button type="button" class="button-empty c-silver-sand">get in touch</button>
                            </div>

                        </div>
                    </div>
                </div>

                <div class="box-link">
                    <ul>
                        <li>
                            <h3>About</h3>
                        </li>
                        <li v-for="(element, index) in linkAbout" :key="index" class="c-silver-sand">
                            <span><i :class="`${element.icon}`"></i></span>
                            <a :href="`${element.href}}`" class="c-silver-sand">{{element.name}}</a>
                        </li>
                    </ul>
                </div>

                <div class="box-link">
                    <ul>
                        <li>
                            <h3>Services</h3>
                        </li>
                        <li v-for="(element, index) in linkServices" :key="index" class="c-silver-sand">
                            <span><i :class="`${element.icon}`"></i></span>
                            <a :href="`${element.href}}`" class="c-silver-sand">{{element.name}}</a>
                        </li>
                    </ul>
                </div>

                <div class="box-link">
                    <ul>
                        <li>
                            <h3>Support</h3>
                        </li>
                        <li v-for="(element, index) in linkSupport" :key="index" class="c-silver-sand">
                            <span><i :class="`${element.icon}`"></i></span>
                            <a :href="`${element.href}}`" class="c-silver-sand">{{element.name}}</a>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
    export default {
        //Cambiare il nome con quello del componente creato
        name: 'FooterLinkComp',
        data() {
            return {
                linkAbout: [{
                        name: 'The company',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Istutional',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Social & Events',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Innovation',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Enviroment',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Technology',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                ],
                linkServices: [{
                        name: 'Audit & Assurance',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Financial Advisory',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Analytics M&A',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Middle Marketing',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Legal Consulting',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Regulatory Risk',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                ],
                linkSupport: [{
                        name: 'Responsability',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Term of use',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'About Cookies',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Privacy Policy',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Accessibility',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
                    },
                    {
                        name: 'Information',
                        icon: 'fa-solid fa-angle-right',
                        href: '#'
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
    .bg-blue-lagoon {
        background-color: $blue-lagoon;
    }

    .bg_image {
        background-image: url(../../assets/img/bg-7.jpg);
        background-size: cover;
        background-position: center;
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

    //fine utility
    ul {
        list-style: none;

        li {
            margin: 10px 0;

            h3 {
                color: #fff;
                margin-bottom: 20px;
                font-size: 1.5em;
            }

            a {
                text-decoration: none;
                margin-left: 10px;
            }
        }
    }
    a:hover{
        color: $fountain-blue;
    }

    .rows {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .button-empty {
        background-color: transparent;
        border: 1px solid $blue-lagoon;
        text-transform: uppercase;
        padding: 10px 20px;
        border-radius: 5px;
        margin-top: 20px;
    }
    .button-empty:hover {
        background-color: $fountain-blue;
        border-color: $fountain-blue;
        color: #fff;
    }

    .info {
        display: flex;
        flex-direction: column;
        margin-top: 40px;
    }

    .box-internal {
        width: 80%;
        margin: 0 auto;
    }

    .box-link {
        background-color: $abbey-01;
        padding: 40px 50px 30px 40px;
        border-radius: 5px;
    }

    h2 {
        text-transform: uppercase;
        font-family: 'Montserrat', sans-serif;
        font-size: 1.1em;
        font-weight: 900;
        letter-spacing: 5px;
    }

    .nex-custom {
        color: $blue-lagoon;
        background-color: $surfiegreen;
        padding: 7px 0px 7px 20px;
        border-radius: 50px 0 0 50px;
    }

    .gen-custom {
        color: $silver-sand;
        margin-left: 3px;
    }
    .logo{
        margin-bottom: 30px;
    }
</style>