<template>
  <div class="container p-4">
       <div class="row">
           <div class="col-4">
              <img src="../assets/img/logo_seo_w_1x.png" alt="logo">
           </div>
           <div class="col-8">
              <a v-for="(link, index) in links" :key="index" href="link.url">{{ link.name }}</a>
              <div class="ms_d-inline ms_btn">
                 <button class="ms_btn_org ms_clr_wht">Get in touch now</button>
              </div>
           </div>
       </div>
  </div>
</template>

<script>
export default {
   name: 'Navbar',

   data: function(){
     return{
        links: [
            {
                name:'Home',
                url:'#',
            },

            {
                name:'Who We Are',
                url:'#',
            },

            {
                name:'What We Do',
                url:'#',
            },

            {
                name:'Where We Work',
                url:'#',
            },

            {
                name:'Careers',
                url:'#',
                btn:'apply'
            },

            {
                name:'News',
                url:'#',
            },
        ]
     }
   }
}
</script>

<style lang="scss">
 a{
    text-decoration: none;
    color: white;
    padding-left: 20px;
    &:hover{
        color: #ffa837;
    }
 }

 .ms_btn{
   padding-left: 40px;
 }

 .ms_d-inline{
    display: inline-block;
 }

 .ms_btn_org{
    text-transform: uppercase;
    background-color: #ffa837;
    border: 0;
    border-radius: 20px;
    padding: 5px 20px;
    font-weight: bold;
    &:hover{
        border: 4px solid #dd9f4d;
    }
 }
</style>