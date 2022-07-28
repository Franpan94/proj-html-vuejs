<template>
  <div class="pt-5 text-center ms_bg_desk">
    <img src="../../assets/img/logo_seo_1x.png" alt="logo" />
    <div class="pt-5 pb-5">
      <a class="ms_b_color" v-for="(link, index) in links" :key="index" :href="link.url">{{
        link.name
      }}</a>
    </div>
    <div>
      <span v-for="(voice,i) in voices" :key="i" class="ms_color_paragraph">
        {{ voice.name }} 
        <span class="ms_b_color">{{ voice.theme }}</span> 
        <span>{{ voice.symbol }}</span>
      </span>
    </div>
    <div>
      <i v-for="(icone, counter) in icones" :class="icone" :key="counter" class="p-2 pt-4 pb-5 icones"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "EndFooter",

  data: function () {
    return {
      links: [
        {
          name: "Home",
          url: "#",
        },

        {
          name: "Who We Are",
          url: "#",
        },

        {
          name: "What We Do",
          url: "#",
        },

        {
          name: "Where We Work",
          url: "#",
        },

        {
          name: "Careers",
          url: "#",
        },

        {
          name: "News",
          url: "#",
        },

        {
          name: "Get in Touch Now",
          url: "#",
        },
      ],

      voices: [
        {
          name: '© Copyright 2012-2020',
          symbol:'|',
        },

        {
          name: 'Avada Theme by',
          theme:'ThemeFusion',
          symbol:'|',
        },

        {
          name: 'All Rights Reserved ',
          symbol:'|',
        },

        {
          name: 'Powered by ',
          theme:'Wordpress',
          symbol:'|',
        },
      ],

      icones: ['fa-brands fa-facebook-f', "fa-brands fa-instagram", "fa-brands fa-twitter", "fa-brands fa-youtube"]
    };
  },
};
</script>

<style lang='scss'>

@import "../../assets/styles/Colors.scss";


.ms_bg_desk {
  background-color: $bg_white_card;
}

.ms_b_color{
  color: $bg_black;
}

.icones{
  color: $clr_grey;
  &:hover{
        color: $btn_org;
        cursor: pointer;
    }
}
</style>