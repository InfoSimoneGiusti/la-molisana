<template>
  <div class="footer-links">
    <h4>{{title}}</h4>
    <ul>
        <li v-for="(url, index) in urls" :key="index">
            <a :href="url.url">{{url.text}}</a>
        </li>
    </ul>
  </div>
</template>

<script>
export default {
    name: "FooterMenu",
    props: {
        title: String,
        urls: Array
    }
}
</script>

<style lang="scss">

    .footer-links {

        h4 {
            margin-bottom: 1rem;
            font-weight: 500;
        }

        ul {
            list-style: none;

            li {

                a {
                    text-decoration: none;
                    font-weight: 300;
                    color: black;
                    line-height: 1.4rem;

                    &:hover {
                        font-weight: 500;
                    }
                }

            
            }
        }
    }

</style>