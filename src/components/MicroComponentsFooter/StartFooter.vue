<template>
  <div class="ms_bg_key">
      <div class="text-center ms_pt_10 ms_clr_wht ms_bg_opacity ">
        <h3 class="ms_font">Start your free consultation</h3>
        <p class="pt-2">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
        <button class="ms_btn_org ms_clr_wht">contact us now</button>
     </div>  
  </div>
</template>

<script>
export default {
  name:'EndFooter'
}
</script>

<style lang="scss">
  .ms_bg_key{
    background-image: url('../../assets/img/bigkeyup.jpg');
    height: 60vh;
    background-size: cover;
    background-position: center;
  }

  .ms_bg_opacity{
      background-color : rgba(0,0,0,0.6);
      height: 60vh;
  }

  .ms_pt_10{
    padding-top: 8.5rem;
  }
</style>