<template>
<div>
   <div class="contenedor">
      <img 
      :src="imagen" 
      alt="" 
      class="avatarImg">
      <p class="nombre"> {{nombre}}</p>
    </div>
 </div>
</template>
<script>

export default {
  props: ["nombre",  "imagen"]
  
}
</script>
<style>
.contenedor{
    text-align: center; 
    margin-bottom: 100px;
  }
  .nombre{
    color: green; 
    font-size: 40px; 
    margin: 0px;
  }
  .avatarImg{
      border-radius: 50%; 
      height:200px;
  }
</style>
