<template>
   <main>
     <NewAgency />
     <NotchServices />
     <OurWork />
     <OurPlans />
     <OurNews />
     <ClientSay />
   </main>
</template>

<script>
import NewAgency from './MicroComponentsMain/NewAgency.vue'
import NotchServices from './MicroComponentsMain/NotchServices.vue'
import OurWork from './MicroComponentsMain/OurWork.vue'
import OurPlans from './MicroComponentsMain/OurPlans.vue'
import OurNews from './MicroComponentsMain/OurNews.vue'
import ClientSay from './MicroComponentsMain/ClientSay.vue'

export default {
  name: 'Main',
  components: {
    NewAgency,
    NotchServices,
    OurWork,
    OurPlans,
    OurNews,
    ClientSay
  }
}
</script>

<style lang="scss">

</style>