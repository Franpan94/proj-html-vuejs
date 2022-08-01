<template>
  <div class="ms_background text-center pt-5 pb-5">
    <h2 class="ms_font ms_clr_wht">Our Plans</h2>
    <p class="pt-2 ms_clr_wht">Sed ut perspiciatis unde omnis iste natus error sit voluptatem <br> accusantium doloremque laudantium</p>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="col-2 pt-3 ms_bg_plan_card pb-4" v-for="plan in plans" :key="plan.id">
          <h2 class="ms_font pb-5">{{ plan.title }}</h2>
          <div class="ms_position_relative pb-4">
            <span class="ms_font ms_pst_abslt1">$</span> 
            <span class="fs-1 ms_font ms_clr_plan">{{ plan.bignumber }}</span> 
            <span class="ms_font_size ms_font ms_pst_abslt2 ms_clr_plan">99</span>
            <span class="ms_font_size ms_font ms_color_paragraph">monthly</span> 
          </div>
          <h6 class="pb-4">{{ plan.proj }}</h6>
          <h6 class="pb-4">{{ plan.stor }}</h6>
          <h6 class="pb-4">Unlimited Users</h6>
          <button class="ms_btn_original">start today</button>
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
          bignumber:'19',
          proj:'5 Project',
          stor:'5 GB Storage',
          id: 0,
        },

        {
          title: "Premium",
          bignumber:'29',
          proj:'10 Project',
          stor:'15 GB Storage',
          id: 1,
        },

        {
          title: "Professional",
          bignumber:'39',
          proj:'15 Project',
          stor:'30 GB Storage',
          id: 2,
        },

        {
          title: "Extreme",
          bignumber:'59',
          proj:'Unlimited Project',
          stor:'Unlimited GB Storage',
          id: 3,
        },
      ],
    };
  },
};
</script>

<style lang="scss">

@import '../../assets/styles/Colors.scss';


.ms_background {
  background-image: url("../../assets/img/background1.jpg");
  height: 100vh;
  background-size: cover;
}

.ms_bg_plan_card{
 background-color: $bg_white_card;
 margin: 10px;
 padding-bottom: 10px;
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
  color: $btn_sky;
}

.ms_btn_original{
    text-transform: uppercase;
    border-radius: 20px;
    padding: 5px 20px;
    font-weight: bold;
    border: 2px solid $bg_black;
    &:hover{
      background-color: $btn_org;
      color: $btn_sky_text;
      border: 0;
    }
  }
</style>