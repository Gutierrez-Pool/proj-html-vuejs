<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  data() {
    return {
      
    }
  },

  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<template>
  <Header></Header>
  <Main></Main>
  <Footer></Footer>
</template>

<style lang="scss">
@use './styles/variables' as *;

Header {
  background: linear-gradient(to top, #01012f 0%, #0b1952 100%);
}

</style>
