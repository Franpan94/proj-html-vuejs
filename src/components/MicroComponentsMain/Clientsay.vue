<template>
  <div class="text-center pt-5 pb-5">
    <h2 class="ms_font">Whatch Our Clients Say</h2>
    <img :src="require(`../../assets/img/${testimonials[i].img}.jpg`)" alt="img" class="pt-3 ms_radius">
    <p class="pt-3">{{ testimonials[i].paragraph }}</p>
    <span class="ms_font">{{ testimonials[i].name }}</span>
    <span class="ms_upper">{{ testimonials[i].work }}</span>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div v-for="(circle,counter) in 2" :key="counter" class="ms_circle" :class="isActivate(counter)"  @click="isActivateImg(counter)"></div>
      </div>
      <div class="row">
        <div class="col-3 mt-5 ms_bord" div v-for="(img,index) in imgs" :key="index">
          <img :src="require(`../../assets/img/${img}.png`)" alt="img" class="mt-5">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Ourwork',

  data: function(){
    return{
      i:0,
      imgs:['avada-flame','the-avada','avada-rombo','avada-law'],
      testimonials: [
        {
          img: 'testimonialman',
          paragraph: 'Ability procedees from a fusion of skills, knowledge, understanding and imagination, consolidated, by experience.',
          name:'Luis Desalvo',
          work:', creo tech',
        },

        {
          img: 'testimonialwoman',
          paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, porro repellat velit accusamus quisquam voluptatibus!',
          name:'Angelina Jolie',
          work:', developer',
        },
      ]
    }
  },

  methods:{
    isActivate(position){
      if(this.i === position){
        return 'ms_active';
      }
    },

    isActivateImg(number){
      this.i = number;
    }
  }
}
</script>

<style lang='scss'>

 @import '../../assets/styles/Colors.scss';

.ms_radius{
  border-radius: 50%;
}

.ms_upper{
  text-transform: uppercase;
}

.ms_active{
 background-color: $bg_black;
}

.ms_circle{
  height: 25px;
  border: 1px solid $bg_black;
  width: 25px;
  border-radius: 50%;
  margin-left: 10px;
  cursor: pointer;
}

.ms_bord{
  border-top: 1px solid $bg_white_card_hover;
}

</style>