<template>
     <div>
          <div class="container">
               <div class="row">
                    <ul>
                         <li
                              v-for="(data, index) in datosPersonajes"
                              :key="index"
                         >
                              <div class="bloque">
                                   <img
                                        :src="data.image"
                                        class=" imagen rounded-circle float-left"
                                        :alt="data.name"
                                   />
                                   <span class="texto">{{ data.name }}</span>
                              </div>
                         </li>
                    </ul>
               </div>
          </div>
     </div>
</template>

<script>
export default {
     name: "Perosnaje",
     props: {
          datosPersonajes: {
               type: Array,
               required: true,
          },
     },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bloque {
     width: 300px;
     height: 150px;
}

.imagen {
     width: 100px;
     height: 100px;
}
.texto {
     color: darkgreen;
     font-size: 25px;
     margin-left: 20px;
     margin-top: 200px;
}
</style>
