<script>
import Navbar from '../components/Navbar.vue';
import Jumbotron from '../components/Jumbotron.vue';

export default {
  data() {
    return {
      
    }
  },

  components: {
    Navbar,
    Jumbotron,
  }
}
</script>


<template>
  <div id="bg-principal">
    <Navbar></Navbar>
    <Jumbotron></Jumbotron>
  </div>
</template>


<style lang="scss">

#bg-principal {
  background: linear-gradient(to top, #01012f 0%, #0b1952 100%);
}

</style>