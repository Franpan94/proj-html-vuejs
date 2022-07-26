<template>
  <div class="text-center pt-5">
    <h2 class="ms_font">Meet The New Agency SEO Template <br> From The Avada Team</h2>
    <p class="pt-2 ms_color_paragraph">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row">
        <div class="col-4 pt-5" v-for="(paragraph,index) in paragraphs" :key="index">
          <i :class="paragraph.img"></i>
          <h3 class="pt-2 ms_font">{{ paragraph.title }}</h3>
          <p class="ms_color_paragraph">{{ paragraph.theme }}</p>
        </div>
        <img src="../assets/img/agency-seo-desk-front.jpg" alt="">
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
                theme:'Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisques convallis, mi ligula eismod odio vel dictum mi risus ami',
                img:'fa-solid fa-water-ladder',
            },

            {
                title:'Who We Are',
                theme:'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Libero ullam, nesciunt soluta consectetur ea dolore.',
                img:'fa-solid fa-video',
            },

            {
                title:'What We Do',
                theme:'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Libero ullam, nesciunt soluta consectetur ea dolore.',
                img:'fa-solid fa-droplet',
            },
        ]
     }
   }
}
</script>

<style lang="scss">

i{
  color: #ffa837;
}

.ms_bg_newagency{
  background-image: url('../assets/img/transparent.png');
}

.ms_font{
  font-weight: bolder;
}

.ms_color_paragraph{
  color: grey;
}
</style>