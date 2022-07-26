<template>
   <header class="ms_bg">
     <Navbar />
   </header>
</template>

<script>
import Navbar from './Navbar.vue'

export default {
   name:'Header',
   components: {
    Navbar,
   }
}
</script>

<style lang="scss" scoped>
  .ms_bg{
    background-image: url('../assets/img/1-hero-image.png');
    height: 100vh;
    background-size: cover;
  }
</style>