<template>
  <div class="pt-5 text-center ms_bg_desk">
    <img src="../../assets/img/logo_seo_1x.png" alt="logo" />
    <div class="pt-5 pb-5">
      <a class="ms_b_color" v-for="link in links" :key="link.id" href="#">{{
        link.name
      }}</a>
    </div>
    <div>
      <span v-for="voice in voices" :key="voice.id" class="ms_color_paragraph">
        {{ voice.name }} 
        <span class="ms_b_color">{{ voice.theme }}</span> 
        <span> | </span>
      </span>
    </div>
    <div>
      <i v-for="icone in icones" :class="icone.img" :key="icone.id" class="p-2 pt-4 pb-5 icones"></i>
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
          id: 0,
        },

        {
          name: "Who We Are",
          id: 1,
        },

        {
          name: "What We Do",
          id: 2,
        },

        {
          name: "Where We Work",
          id: 3,
        },

        {
          name: "Careers",
          id: 4,
        },

        {
          name: "News",
          id: 5,
        },

        {
          name: "Get in Touch Now",
          id: 6,
        },
      ],

      voices: [
        {
          name: '© Copyright 2012-2020',
          id: 0,
        },

        {
          name: 'Avada Theme by',
          theme:'ThemeFusion',
          id: 1,
        },

        {
          name: 'All Rights Reserved ',
          id: 2,
        },

        {
          name: 'Powered by ',
          theme:'Wordpress',
          id: 3,
        },
      ],

      icones: [
        {
          img:'fa-brands fa-facebook-f', 
          id: 0,
        },

        {
          img: "fa-brands fa-instagram", 
          id: 1,
        },

        {
          img: "fa-brands fa-twitter", 
          id: 2,
        },

        {
          img: "fa-brands fa-youtube",
          id: 3,
        },
      ]
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