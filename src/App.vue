<template>
  <div id="app">
    <MyHeader/>
    <MyProducts/>
    <MyFooter/>

    <div class='provaCentratura'>PROVA</div>

  </div>
</template>

<script>

import MyHeader from './components/MyHeader';
import MyProducts from './components/MyProducts';
import MyFooter from './components/MyFooter';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyProducts,
    MyFooter
  }
}
</script>

<style lang="scss">

  @import './styles/general.scss';
  @import './styles/vars.scss';
  @import './styles/typo.scss';
  @import './styles/utilities.scss';
  @import '~bootstrap/scss/bootstrap.scss';

  @import './styles/mixins.scss';

  h1, h2, h3, h4, h5, h6 {
      color: $brand_color;
  }

  .provaCentratura {
    background: grey;
    height: 400px;
    @include centra('orizzontale');
  }
</style>
