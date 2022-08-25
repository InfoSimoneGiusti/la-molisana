<template>
    <div class="product-card">
        <img :src="imageSrc" />
        <h3>{{title}}</h3>
    </div>
</template>

<script>
export default {
    name: "SingleProduct",
    props: {
        imageSrc: String,
        title: String
    }
}
</script>

<style lang="scss">

    .product-card {

        flex-basis: 25%;
        background-color: white;
        padding: 10px;
        border: solid 2px #DBE7FF;

        img {
            max-width: 100%;
        }

        h3 {
            font-size: 16px;
        }

    }

</style>