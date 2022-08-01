<template>
  <div class="text-center pt-5 ms_bg_white">
    <h2 class="ms_font">Meet The New Agency SEO Template <br> From The Avada Team</h2>
    <p class="pt-2 ms_color_paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-3 pt-3 pb-2 ms_bg_white_card" v-for="paragraph in paragraphs" :key="paragraph.id">
          <i :class="paragraph.img"></i>
          <h3 class="pt-2 ms_font">{{ paragraph.title }}</h3>
          <p class="ms_color_paragraph">{{ paragraph.theme }}</p>
        </div>
        <img src="../../assets/img/agency-seo-desk-front.jpg" alt="img" class="pt-5" >
      </div>
    </div>
  </div>
</template>

<script>
export default {
   name: 'Newagency',

   data: function(){
     return{
        paragraphs: [
            {
                title:'Establish Goals',
                theme:'Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisques convallis, mi ligula eismod odio vel dictum mi risus ami.',
                img:'fa-solid fa-water-ladder',
                id: 0,
            },

            {
                title:'Work With a Team',
                theme:'Cras semper auctor aliquam. Sed porta sed lacus sit amet consectetur. Lorem ipsum dolor sit amet consectetur adipiscin.',
                img:'fa-solid fa-video',
                id: 1,
            },

            {
                title:'Get Results',
                theme:'Vestibulum scelerisque egestas lectus sit amet molestie. Donec consectetur cursus est sed blandit. Nunc sed risus lacus.',
                img:'fa-solid fa-droplet',
                id: 2,
            },
        ]
     }
   }
}
</script>

<style lang="scss">

 @import '../../assets/styles/Colors.scss';


i{
  color: $btn_org;
}

.ms_bg_newagency{
  background-image: url('../../assets/img/transparent.png');
}

.ms_font{
  font-weight: bolder;
}

.ms_color_paragraph{
  color: $clr_grey;
}

.ms_bg_white{
  background-color: $btn_sky_text;
}

.ms_bg_white_card{
 background-color: $bg_white_card;
 margin: 10px;
 padding-bottom: 10px;
 &:hover{
  border: 8px solid $bg_white_card_hover;
  cursor: pointer;
 }
}
</style>