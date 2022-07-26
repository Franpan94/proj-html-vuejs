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
import Newagency from './Newagency.vue'
import Notchservices from './Notchservices.vue'
import Ourwork from './Ourwork.vue'
import Ourplans from './Ourplans.vue'
import Ournews from './Ournews.vue'
import Clientsay from './Clientsay.vue'

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

<style>

</style>