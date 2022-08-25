<template>
    <footer>

        <div class="cols container">
            <a href="#" class="footer-logo">
                <img :src="require('../assets/images/la-molisana-logo.png')" />
            </a>

            <FooterMenu :title="'PASTIFICIO'" :urls="pastificioUrls" />
            <FooterMenu :title="'PRODOTTI'" :urls="prodottiUrls" />
           
        </div>    

        <img class="footer-img" src='@/assets/images/footer-montagne-bottom.jpg' />
    </footer>
</template>

<script>

import FooterMenu from './FooterMenu.vue';

export default {
    name: 'MyFooter',
    components: {
        FooterMenu
    },
    data() {
        return {
            pastificioUrls: [
                                {
                                    url: '#',
                                    text: 'Il Pastificio'
                                },
                                {
                                    url: '#',
                                    text: 'Grano'
                                },
                                {
                                    url: '#',
                                    text: 'Filiera'
                                },
                                {
                                    url: '#',
                                    text: '100 anni di pasta'
                                },
                                {
                                    url: '#',
                                    text: 'Sartoria della pasta'
                                },
                                {
                                    url: '#',
                                    text: 'Bla Bla Bla'
                                },
                            ],
            prodottiUrls: [
                                {
                                    url: '#',
                                    text: 'Le classiche'
                                },
                                {
                                    url: '#',
                                    text: 'Le integrali'
                                },
                                {
                                    url: '#',
                                    text: 'Le speciali'
                                },
                                {
                                    url: '#',
                                    text: 'Le biologiche'
                                },
                                {
                                    url: '#',
                                    text: 'Senza glutine'
                                },
                            ]
        }
    }
}
</script>

<style scoped lang="scss">

    @import '../styles/mixins.scss';

    .footer-img {
        max-width: 100%;
    }
    .cols {
        @include centra('orizzontale');

        .footer-logo {
            margin: 5rem 0 2rem;
        }
        .footer-links {
            margin: 5rem 5rem 2rem 5rem;
        }
        
    }

</style>