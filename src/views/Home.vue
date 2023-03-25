<template>
  <v-layout class="mt-3">
    <v-row class="clickable">
      <v-col cols="12" md="12">
        <v-card class="ml-5 mr-5">
          <v-app-bar  
            dark
            color="#2c3a47"
          >
                <v-btn  icon>  
                  <v-icon>mdi-home</v-icon>
                </v-btn>
                <v-toolbar-title>Dashboard</v-toolbar-title>
          </v-app-bar>
          <v-container>
            <v-row>
              <v-col cols="12" sm="4">
                <v-hover v-slot:default="{hover}"
                open-delay="200"
                >
                  <v-card
                    :elevation="hover?16:2"
                    class="mx-auto"
                    max-width="344"
                    outlined
                  >
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-list-item-title class="headline mb-1">Orders</v-list-item-title>
                      </v-list-item-content>
                      <v-list-item-avatar
                        tile 
                        size="80"
                        color="red darken-2"
                      >
                        <v-icon dark> fas fa-box-open</v-icon>
                      </v-list-item-avatar>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-card-actions>
                      <v-icon flab color="red darken-2">local_offer</v-icon>
                      <v-btn text >243k</v-btn>
                      <v-spacer></v-spacer>
                      <v-icon flab color="#2c3a47">mdi-chevron-right</v-icon>

                    </v-card-actions>
                  </v-card>
                </v-hover>
              </v-col>
              <v-col cols="12" sm="4">
                <v-hover v-slot:default="{hover}"
                  open-delay="200"
                  >
                  <v-card
                    :elevation="hover?16:2"
                    class="mx-auto"
                    max-width="344"
                    outlined
                  >
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-list-item-title class="headline mb-1">Sales</v-list-item-title>
                      </v-list-item-content>
                      <v-list-item-avatar
                        tile 
                        size="80"
                        color="#009432"
                      >
                        <v-icon dark> mdi-watch</v-icon>
                      </v-list-item-avatar>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-card-actions>
                      <v-icon flab color="#009432">directions_walk</v-icon>
                      <v-btn text >243k</v-btn>
                      <v-spacer></v-spacer>
                      <v-icon flab color="#2c3a47">mdi-chevron-right</v-icon>

                    </v-card-actions>
                  </v-card>
                </v-hover>
              </v-col>              
              <v-col cols="12" sm="4">
                <v-hover v-slot:default="{hover}"
                  open-delay="200"
                  >
                  <v-card
                    :elevation="hover?16:2"
                    class="mx-auto"
                    max-width="344"
                    outlined
                  >
                    <v-list-item three-line>
                      <v-list-item-content>
                        <v-list-item-title class="headline mb-1">Devices</v-list-item-title>
                      </v-list-item-content>
                      <v-list-item-avatar
                        tile 
                        size="80"
                        color="#f79f1f"
                      >
                        <v-icon dark> fas fa-laptop-house</v-icon>
                      </v-list-item-avatar>
                    </v-list-item>
                    <v-divider></v-divider>
                    <v-card-actions>
                      <v-icon flab color="#f79f1f">description</v-icon>
                      <v-btn text >243k</v-btn>
                      <v-spacer></v-spacer>
                      <v-icon flab color="#2c3a47">mdi-chevron-right</v-icon>

                    </v-card-actions>
                  </v-card>
                </v-hover>
              </v-col>
             
            </v-row>
          </v-container>
        </v-card>
      </v-col>
      <h1 class="py-3 mx-3" >
        <Carousel/>
      </h1>
    </v-row> 
  </v-layout>
</template>

<script>
// @ is an alias to /src
import Carousel from "../components/Carousel.vue";
export default {
  name: 'Home',
  components: {
    Carousel
  }
}
</script>
