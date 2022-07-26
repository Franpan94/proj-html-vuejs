<template>
  <div>
    ciao notch
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
                links: [
                  {
                    name: 'Read More'
                    image: ''
                  }
                ]
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

<style>

</style>