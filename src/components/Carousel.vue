<template>
    <v-sheet
    class="mx-auto"
    elevation="8"
    max-width="800"
  >
    <v-slide-group
      v-model="model"
      class="pa-4"
      active-class="success"
      show-arrows
    >
      <v-slide-item
        v-for="(slide, i) in slides"
        :key="i"
        v-slot="{ active, toggle }"
      >
        <v-card
          :color="active ? undefined : 'grey lighten-1'"
          class="ma-4"
          height="200"
          width="100"
          @click="toggle"
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <v-img :src="slide.src"></v-img>
            
            <v-scale-transition>
              <v-icon
                v-if="active"
                color="white"
                size="48"
                v-text="'mdi-close-circle-outline'"
              ></v-icon>
            </v-scale-transition>
          </v-row>
        </v-card>
      </v-slide-item>
    </v-slide-group>
  </v-sheet>
</template>


<script>

    export default {
        data() {
            return {
                slides: [
                    {src: '01.jpg'},                        
                    {src: '02.jpg'},                        
                    {src: '03.jpg'},                       
                    {src: '04.jpg'},                      
                    {src: '05.jpg'},                     
                    {src: '06.jpg'},                    
                    {src: '07.jpg'},                   
                    {src: '08.jpg'},                  
                    {src: '09.jpg'},                     
                    {src: '10.jpg'}                            
                ]
            }
        },
    }
</script>


<style>
    .carousel-3d-slide{
        height: 100% !important;
    }
</style>