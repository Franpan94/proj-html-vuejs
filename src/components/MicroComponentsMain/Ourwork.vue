<template>
  <div class="text-center pt-5 pb-5">
    <h2 class="ms_font">Our Work</h2>
    <p class="pt-2 ms_color_paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row">
        <div class="col-4" v-for="(img,index) in imgs" :key="index">
          <img :src="require(`../../assets/img/${img}.jpg`)" alt="img" class="mt-4">
        </div>
      </div>
      <div class="pt-5">
        <button class="ms_btn_org ms_clr_wht">view our work</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Ourwork',

  data: function(){
    return{
      imgs:['computer','analytics','dates','users','score','click']
    }
  },
}
</script>

<style>

</style>