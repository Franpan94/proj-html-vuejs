<template>
  <div class="text-center pt-5 ms_bg_blu ms_clr_wht ms_bg_img">
    <h2 class="ms_font">See Our Top Notch Services</h2>
    <p class="pt-2">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="col-2 pt-3 ms_bg_card" v-for="paragraph in paragraphs" :key="paragraph.id">
          <i :class="paragraph.img" class="pt-3"></i>
          <h4 class="pt-2 ms_font">{{ paragraph.title }}</h4>
          <p class="ms_clr_wht pt-1">Vestibulum in lacinia metus. Suspendisse in enim ipsum. NUlla facilissi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.</p>
          <div class="pb-2 ms_pr-2">
            <a href="#">Read More</a>
            <i class="fa-solid fa-angle-right ms_pl-05 ms__cursor"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Notchservices",

  data: function () {
    return {
      paragraphs: [
        {
          title: "Google SEO",
          img: "fa-brands fa-google",
          id: 0,
        },

        {
          title: "Brand Strategy",
          img: "fa-solid fa-gear",
          id: 1,
        },

        {
          title: "Local SEO",
          img: "fa-solid fa-house",
          id: 2,
        },

        {
          title: "SEO Analysis",
          img: "fa-solid fa-chart-bar",
          id: 3,
        },
      ],
    };
  },
};
</script>

<style lang="scss">

 @import '../../assets/styles/Colors.scss';


.ms_bg_blu{
  background-color: $bg_blu;
}

.ms_bg_card{
  background-color: $btn_sky_over;
  margin: 10px;
  padding-bottom: 10px;
}

.ms_bg_img{
  background-image: url('../../assets/img/pattern_background.png');
  background-size: cover;
  height: 100vh;
}

.ms_pr-2{
  padding-right: 20px;
}

.ms_pl-05{
  padding-left: 5px;
}

.ms__cursor{
  cursor: pointer;
}
</style>