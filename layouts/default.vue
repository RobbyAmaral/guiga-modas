<template>
  <div>
    <Header />
    <nuxt />
    <Footer />
  </div>
</template>
<script>
import Header from '~/components/Navigator/Header';
import Footer from '~/components/Footer';

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
* {margin:0; padding: 0; text-decoration: none;}
html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
  ul, li, a {
    display: block;
  }
}
</style>
