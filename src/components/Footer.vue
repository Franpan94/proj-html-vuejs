<template>
  <footer>
    <StartFooter />
    <EndFooter />
  </footer>
</template>

<script>
import StartFooter from './MicroComponentsFooter/StartFooter.vue'
import EndFooter from './MicroComponentsFooter/EndFooter.vue'

export default {
   name: 'Footer',
   components: {
    StartFooter,
    EndFooter
   }
}
</script>

<style lang="scss">

</style>