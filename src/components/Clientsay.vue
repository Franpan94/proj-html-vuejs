<template>
  <div class="text-center pt-5 pb-5">
    <h2 class="ms_font">Whatch Our Clients Say</h2>
    <img src="../assets/img/testimonials-2.jpg" alt="img" class="pt-3 ms_radius">
    <p class="pt-3">Ability procedees from a fusion of skills, knowledge, understanding and imagination, <br> consolidated, by experience.</p>
    <span class="ms_font">Luis Desalvo</span>
    <span class="ms_upper">, creo tech</span>
    <div class="container">
      <div class="row justify-content-center pt-5">
        <div class="ms_circle"></div>
        <div class="ms_circle_empty"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang='scss'>

.ms_radius{
  border-radius: 50%;
}

.ms_upper{
  text-transform: uppercase;
}

.ms_circle{
  height: 25px;
  background-color: black;
  width: 25px;
  border-radius: 50%;
}

.ms_circle_empty{
  height: 25px;
  border: 1px solid black;
  width: 25px;
  border-radius: 50%;
  margin-left: 10px;
}

</style>