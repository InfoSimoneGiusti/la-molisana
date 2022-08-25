<template>
  <img :src="percorsoProva" />
</template>

<script>
export default {
    name: 'ComponenteProva',
    data() {
        return {
            percorsoProva: require('../assets/images/prova.jpg')
        }
    }
}
</script>

<style>

</style>