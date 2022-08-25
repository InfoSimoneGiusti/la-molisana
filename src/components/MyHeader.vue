<template>
  <header>
    <img src="@/assets/images/la-molisana-logo.png">
    <nav>
        <ul>
            <li v-for="(link, index) in pincopallino" :key="index" >
                <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
            </li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'MyHeader',
    props: {
        pincopallino: Array
    }
}
</script>

<style lang="scss">

    @import '../styles/vars.scss';

    header {
        text-align: center;
        padding-bottom:20px;

        ul {
            list-style: none;
            margin: 20px;

            li {
                display: inline-block;
                margin: 0px 5px;

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
