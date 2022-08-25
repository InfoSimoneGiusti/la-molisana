<template>
  <h1>{{informazioni.nome}} - {{informazioni.cognome}} - {{informazioni.eta}}</h1>
</template>

<script>
export default {
    name: 'ProvaPassaggioDati',
    //props: ['testo', 'numero']
    props: {
        informazioni: Object,
    }
}
</script>

<style>

</style>