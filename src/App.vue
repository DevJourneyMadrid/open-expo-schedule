<template>
  <div id="app">
    <NavHeader/>
    <Layout>
      <template slot="main">
        <router-view/>
      </template>
      <template slot="footer">
        <FooterLinks></FooterLinks>
      </template>
    </Layout>
  </div>
</template>

<style lang="stylus">
  #app
    font-family 'Avenir', Helvetica, Arial, sans-serif
    -webkit-font-smoothing antialiased
    -moz-osx-font-smoothing grayscale
    color #2c3e50


</style>

<script>
  import NavHeader from './components/NavHeader.vue';
  import FooterLinks from './components/FooterLinks.vue';
  import Layout from './layouts/main.vue';

  export default {
    components: {
      Layout,
      NavHeader,
      FooterLinks,
    },
  };
</script>

<style lang="stylus">
  .la-img img
    height 200px
  @media (max-width: 767.98px)
    .la-img img
      width 100%
      height auto

  .la-img2 img
    max-height 500px
    max-width 100%
  @media (max-width: 767.98px)
    .la-img2 img
      width 100%
      height auto
</style>
