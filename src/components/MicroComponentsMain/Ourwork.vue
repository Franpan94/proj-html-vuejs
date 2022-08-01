<template>
  <div class="text-center pt-5 pb-5">
    <h2 class="ms_font">Our Work</h2>
    <p class="pt-2 ms_color_paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row">
        <div class="col-4" v-for="img in imgs" :key="img.id">
          <img :src="require(`../../assets/img/${img.img}.jpg`)" :alt="img.name" class="mt-4">
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
      imgs:[
        {
          img:'computer',
          name: 'computer',
          id: 0,
        },

        {
          img:'analytics',
          name: 'analytics',
          id: 1,
        },

        {
          img:'dates',
          name: 'dates',
          id: 2,
        },

        {
          img:'users',
          name: 'users',
          id: 3,
        },

        {
          img:'score',
          name: 'score',
          id: 4,
        },

        {
          img:'click',
          name: 'click',
          id: 5,
        },
      ]
    }
  },
}
</script>

<style>

</style>