<template>
  <div class="text-center pt-5 pb-5 ms_bg_white">
    <h2 class="ms_font">Our News</h2>
    <p class="pt-2 ms_color_paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="col-4 pt-3 pb-4" v-for="element in news" :key="element.id">
          <img :src="require(`../../assets/img/${element.img}.jpg`)" alt="img" class="ms_width">
          <h4 class="pt-2 ms_font ms_color-orange">{{ element.title }}</h4>
          <h6 class="ms_font_size pb-2">November 1st, 2017</h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae laborum velit consequuntur perferendis incidunt veritatis deleniti illum ullam.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Ournews",

  data: function () {
    return {
      news: [
        {
          img:'apple2',
          title:'Why You Need A SEO Agency Now',
          id: 0,
        },

        {
          img:'coffee2',
          title:'SEO Tips For Your Startup',
          id: 1,
        },

        {
          img:'tablet2',
          title:'Image Optimization For Your Site',
          id: 2,
        },
      ],
    };
  },
}
</script>

<style lang='scss'>

@import '../../assets/styles/Colors.scss';

.ms_width{
  width: 420px;
}

.ms_color-orange{
  color: $btn_org;
}

</style>