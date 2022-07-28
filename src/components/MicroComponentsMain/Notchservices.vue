<template>
  <div class="text-center pt-5 ms_bg_blu ms_clr_wht ms_bg_img">
    <h2 class="ms_font">See Our Top Notch Services</h2>
    <p class="pt-2">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="col-2 pt-3 ms_bg_card" v-for="(paragraph,index) in paragraphs" :key="index">
          <i :class="paragraph.img" class="pt-3"></i>
          <h4 class="pt-2 ms_font">{{ paragraph.title }}</h4>
          <p class="ms_clr_wht">{{ paragraph.theme }}</p>
          <div v-for="(element, i) in paragraph.links" :key="i" class="pb-2">
            <a :href="element.url">{{ element.name }} <i :class="element.image"></i></a>
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
          theme: 'Vestibulu in lacinia metus. Suspendisse in enim ipsum. NUlla facilissi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.',
          img: "fa-brands fa-google",
          links: [
            {
              name: "Read More",
              image: "fa-solid fa-angle-right",
              url: "#",
            },
          ],
        },

        {
          title: "Brand Strategy",
          theme:'Vestibulu in lacinia metus. Suspendisse in enim ipsum. NUlla facilissi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.',
          img: "fa-solid fa-gear",
          links: [
            {
              name: "Read More",
              image: "fa-solid fa-angle-right",
              url: "#",
            },
          ],
        },

        {
          title: "Local SEO",
          theme: 'Vestibulu in lacinia metus. Suspendisse in enim ipsum. NUlla facilissi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.',
          img: "fa-solid fa-house",
          links: [
            {
              name: "Read More",
              image: "fa-solid fa-angle-right",
              url: "#",
            },
          ],
        },

        {
          title: "SEO Analysis",
          theme:'Vestibulu in lacinia metus. Suspendisse in enim ipsum. NUlla facilissi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.',
          img: "fa-solid fa-chart-bar",
          links: [
            {
              name: "Read More",
              image: "fa-solid fa-angle-right",
              url: "#",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss">

 @import '../../assets/styles/ColorsHeader.scss';
 @import '../../assets/styles/ColorsMain.scss';

.ms_bg_blu{
  background-color: $bg_blu;
}

.ms_bg_card{
  background-color: $btn_sky_over;
  margin: 10px;
  padding-bottom: 10px;
  height: 320px;
  &:hover{
  border: 8px solid $btn_sky;
  cursor: pointer;
  }
}

.ms_bg_img{
  background-image: url('../../assets/img/pattern_background.png');
  background-size: cover;
  height: 100vh;
}
</style>