<template>
  <div class="mt-7">
    <p class="text-h5 font-weight-bold">Dev Enviroment Services</p>
    <p class="text-caption mt-n3 grey--text">Your current development enviroment on internal network</p>

    <v-row class="" align="center"   justify="center">
      <v-col cols="12" xl="8" lg="8">
        <v-card elevation="1" class="pa-6">
          <p class="text-h5 font-weight-bold">Server Status</p>
          <p class="text-caption mt-n2"><v-icon size="15">mdi-server</v-icon> Server-BRAVO-192.167</p>
          <v-row no-gutters >
            <v-col cols="12" xl="5" lg="5">
                <v-row align="center" justify="start" no-gutters>
                    <v-col class=" pr-2"  cols="6">
                      <v-card class="pa-2" flat  style="height:30vh;background-color:#C9F4EF;border-radius:15px">

                          <v-row  align="center" justify="center" no-gutters>
                            <p  class="text-caption mt-2">Settings</p>
                            <v-spacer></v-spacer>
                            <v-btn class="mt-n1" icon text plain><v-icon>mdi-dots-vertical</v-icon></v-btn>
                          </v-row>
                      </v-card>
                    </v-col>
                    <v-col class="pl-2"   cols="6">
                      <v-card flat  style="height:30vh;background-color:#FBBFC2;border-radius:15px">

                      </v-card>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12"></v-col>
            
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="12" xl="4" lg="4">
        <v-card flat class="pa-2">
          dkdk
        </v-card>
      </v-col>
    </v-row>

  </div>
</template>

<script>
  

  export default {
    name: 'Home',

    components: {
     
    },
  }
</script>
