<template>
     <div>
          <Personaje :datosPersonajes="infoPersonaje" />
     </div>
</template>

<script>
import Personaje from "./components/Personaje.vue";

export default {
     name: "App",
     data() {
          return {
               infoPersonaje: [
                    {
                         name: "Rick Sanchez",
                         image:
                              "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
                    },
                    {
                         name: "Morty Smith",
                         image:
                              "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
                    },
                    {
                         name: "Summer Smith",
                         image:
                              "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
                    },
                    {
                         name: "Beth Smith",
                         image:
                              "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
                    },
                    {
                         name: "Jerry Smith",
                         image:
                              "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
                    },
               ],
          };
     },
     components: {
          Personaje,
     },
};
</script>

<style scoped>
</style>
