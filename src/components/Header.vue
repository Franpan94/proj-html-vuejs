<template>
   <header class="ms_bg ms_position_relative">
     <Navbar />
     <div class="ms_clr_wht ms_position_absolute">
         <h1>SEM Campaigns Made <br> Simple With Avada</h1>
         <p class="pt-2">Lorem ipsum dolor, sit amet consectetur adipisicing elit. <br> Libero ullam, nesciunt soluta consectetur ea dolore.</p>
         <div class="ms_d-inline p-2">
              <button class="ms_btn_org ms_clr_wht">buy avada now</button>
         </div>
         <div class="ms_d-inline">
             <button class="ms_btn_sky ms_clr_wht">contact us</button>
         </div>
     </div>
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

<style lang="scss">
  .ms_bg{
    background-image: url('../assets/img/1-hero-image.png');
    height: 100vh;
    background-size: cover;
  }

  .ms_btn_sky{
    text-transform: uppercase;
    background-color: #0369d7;
    border: 0;
    border-radius: 20px;
    padding: 5px 20px;
    font-weight: bold;
  }

  .ms_clr_wht{
    color: white;
  }

  .ms_position_relative{
    position: relative;
  }

   .ms_position_absolute{
    position: absolute;
    top: 35%;
    left: 25%
  }
</style>