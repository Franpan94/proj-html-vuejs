<template>
   <main>
     <Newagency />
     <Notchservices />
     <Ourwork />
     <Ourplans />
     <Ournews />
     <Clientsay />
   </main>
</template>

<script>
import Newagency from './MicroComponentsMain/Newagency.vue'
import Notchservices from './MicroComponentsMain/Notchservices.vue'
import Ourwork from './MicroComponentsMain/Ourwork.vue'
import Ourplans from './MicroComponentsMain/Ourplans.vue'
import Ournews from './MicroComponentsMain/Ournews.vue'
import Clientsay from './MicroComponentsMain/Clientsay.vue'

export default {
  name: 'Main',
  components: {
    Newagency,
    Notchservices,
    Ourwork,
    Ourplans,
    Ournews,
    Clientsay
  }
}
</script>

<style lang="scss">

</style>