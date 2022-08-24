<template>
  <header>
    <img src="@/assets/images/la-molisana-logo.png">
    <nav>
        <ul>
            <li v-for="(link, index) in links" :key="index" >
                <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
            </li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            links: [
                {
                    text: 'Home',
                    url: '#',
                    active: false
                },
                {
                    text: 'Prodotti',
                    url: '#',
                    active: true
                },
                {
                    text: 'Chi Siamo',
                    url: '#',
                    active: false
                },
                {
                    text: 'Contatti',
                    url: '#',
                    active: false
                },
                {
                    text: 'Blog',
                    url: '#',
                    active: false
                }
            ]
        }
    }
}
</script>

<style lang="scss">

    @import '../styles/vars.scss';

    header {
        text-align: center;

        ul {
            list-style: none;
            margin: 20px;

            li {
                display: inline-block;
                margin: 0px 10px;

                a {

                    color: black;
                    text-decoration: none;
                    padding:10px;

                    &.active, &:hover {
                        background-color: $selection_color;
                    }

                }
            }
        }
    }

</style>
