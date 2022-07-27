<template>
  <div class="ms_background text-center pt-5 pb-5">
    <h2 class="ms_font ms_clr_wht">Our Work</h2>
    <p class="pt-2 ms_clr_wht">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="col-2 pt-3 ms_bg_plan_card pb-4" v-for="(plan,index) in plans" :key="index">
          <h2 class="ms_font pb-5">{{ plan.title }}</h2>
          <div class="ms_position_relative pb-4">
            <span class="ms_font ms_pst_abslt1">{{ plan.symbol }}</span> 
            <span class="fs-1 ms_font ms_clr_plan">{{ plan.bignumber }}</span> 
            <span class="ms_font_size ms_font ms_pst_abslt2 ms_clr_plan">{{ plan.smallnumber }}</span>
            <span class="ms_font_size ms_font ms_color_paragraph">{{ plan.type }} </span> 
          </div>
          <h6 class="pb-4">{{ plan.proj }}</h6>
          <h6 class="pb-4">{{ plan.stor }}</h6>
          <h6 class="pb-4">{{ plan.users }}</h6>
          <button class="ms_btn_original">{{ plan.butt }}</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Ourplans",

  data: function () {
    return {
      plans: [
        {
          title: "Standard",
          symbol: "$",
          bignumber:'19',
          smallnumber:'99',
          type: 'monthly',
          proj:'5 Project',
          stor:'5 GB Storage',
          users:'Unlimited Users',
          butt: 'start today',
        },

        {
          title: "Premium",
          symbol: "$",
          bignumber:'29',
          smallnumber:'99',
          type: 'monthly',
          proj:'10 Project',
          stor:'15 GB Storage',
          users:'Unlimited Users',
          butt: 'start today',
        },

        {
          title: "Professional",
          symbol: "$",
          bignumber:'39',
          smallnumber:'99',
          type: 'monthly',
          proj:'15 Project',
          stor:'30 GB Storage',
          users:'Unlimited Users',
          butt: 'start today',
        },

        {
          title: "Extreme",
          symbol: "$",
          bignumber:'59',
          smallnumber:'99',
          type: 'monthly',
          proj:'Unlimited Project',
          stor:'Unlimited GB Storage',
          users:'Unlimited Users',
          butt: 'start today',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.ms_background {
  background-image: url("../assets/img/background1.jpg");
  height: 100vh;
  background-size: cover;
}

.ms_bg_plan_card{
 background-color: #f8f8f8;
 margin: 10px;
 padding-bottom: 10px;
 &:hover{
  border: 2px solid #1a236c;
  cursor: pointer;
 }
}

.ms_font_size{
  font-size: 12px;
}

.ms_pst_abslt1{
  position: absolute;
  top: .5rem;
  left: 2.6rem;
}

.ms_pst_abslt2{
  position: absolute;
  top: .6rem;
  left: 6rem;
}

.ms_clr_plan{
  color: #0369d7;
}

.ms_btn_original{
    text-transform: uppercase;
    border-radius: 20px;
    padding: 5px 20px;
    font-weight: bold;
    border: 2px solid black;
    &:hover{
      background-color: #ffa837;
      color: white;
      border: 0;
    }
  }
</style>