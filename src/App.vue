<template>
 <div>
   <div class="logo">
     <img src="assets/logo.png" alt="logo">
   </div>
   <Avatar 
    v-for="(personaje, $index) of personajes" 
    :key="$index" 
    :nombre="personaje.nombre" 
    :imagen="personaje.src"
    />
 </div>
</template>

<script>
import Avatar from '@/components/Avatar.vue'
export default {
  name: 'App',
  components: { Avatar },
  data:() => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
           
      },
      {
        nombre: "Summer Smith",
        scr: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
      {
        nombre: "Abadango Cluster Princess",
        src: "https://rickandmortyapi.com/api/character/avatar/6.jpeg",
      },
      {
        nombre: "Abradolf Lincler",
        src: "https://rickandmortyapi.com/api/character/avatar/7.jpeg",
      },
      {
        nombre: "Adjudicator Rick",
        src: "https://rickandmortyapi.com/api/character/avatar/8.jpeg",
      },
      {
        nombre: "Agency Director",
        src: "https://rickandmortyapi.com/api/character/avatar/9.jpeg",
           
        },
        {
        nombre: "Alan Rails",
        src: "https://rickandmortyapi.com/api/character/avatar/10.jpeg",
        },
        {
        nombre: "Albert Einstein",
        src: "https://rickandmortyapi.com/api/character/avatar/11.jpeg",
        },
    ],
  })
}

</script>

<style>
  body{
    padding: 0;
    margin: 0;
    width: 100%;
    background-image: url('../public/assets/background.png');
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    
  }
  .logo{
    text-align: center;
    width: 100%;
  }
  .logo img{
    width: 100%;
    max-width: 800px;
  }

  
</style>
