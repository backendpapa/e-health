<template>
  <div class="mt-7">
    <p class="text-h5 font-weight-bold">Dev Enviroment Services</p>
    <p class="text-caption mt-n3 grey--text">Your current development enviroment on internal network</p>

    <v-row class="" align="center"   justify="center" no-gutters>
      <v-col cols="12" xl="7" lg="7" class="" >
        <v-card elevation="1" class="pa-4 ma-2">
          <p class="text-h5 font-weight-bold">Server Status</p>
          <v-row class="mb-n2" no-gutters>
         <v-col cols="5">
            <p class="text-caption mt-n2"><v-icon size="15">mdi-server</v-icon> Server-BRAVO-192.167</p>
            
         </v-col>
         <v-col cols="1" />
         <v-col cols="6" >
            <p class="text-caption mt-n2 d-none d-sm-flex"><v-icon size="15">mdi-database-settings-outline</v-icon> Server Account Quote</p>
         </v-col>
            </v-row>
          <v-row no-gutters >
            <v-col cols="12" xl="5" lg="5">
                <v-row align="center" justify="start" no-gutters>
                    <v-col class=" pr-2"  cols="6">
                      <v-card class="pa-2 " flat  style="height:30vh;background-color:#C9F4EF;border-radius:15px">

                          <v-row  align="center" justify="center" no-gutters>
                            <p style="color:#484C87" class="text-caption font-weight-bold mt-2">Settings</p>
                            <v-spacer></v-spacer>
                            <v-btn class="mt-n1" icon text plain><v-icon style="color:#484C87">mdi-dots-vertical</v-icon></v-btn>
                          </v-row>
                          <div style="position:absolute;bottom:0">
                            <p class="text-h4 font-weight-bold" style="color:#484C87">24</p>
                            <p class="mt-n3 text-caption font-weight-bold" style="color:#484C87">Running <br> Services</p>
                          </div>
                      </v-card>
                    </v-col>
                    <v-col class="pl-2"   cols="6">
                      <v-card flat class="pa-2"  style="height:30vh;background-color:#FBBFC2;border-radius:15px">
                           <v-row  align="center" justify="center" no-gutters>
                            <p style="color:#484C87"  class="text-caption font-weight-bold mt-2">Settings</p>
                            <v-spacer></v-spacer>
                            <v-btn class="mt-n1" icon text plain><v-icon style="color:#484C87">mdi-dots-vertical</v-icon></v-btn>
                          </v-row>

                           <div style="position:absolute;bottom:0">
                            <p class="text-h4 font-weight-bold" style="color:#484C87">2</p>
                            <p class="mt-n3 text-caption font-weight-bold" style="color:#484C87">Crashed <br> Services</p>
                          </div>
                      </v-card>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12" xl="1" lg="1" />
            <v-col cols="12" xl="6" lg="6" class="">
              
              <p class="text-caption d-flex d-sm-none mt-3"><v-icon size="15">mdi-database-settings-outline</v-icon> Server Account Quote</p>
              <v-card class="pa-2" flat style="height:30vh;background-color:#F3F5FD;border-radius:15px">
                  <p class="text-caption">Available 32.03GB from 120GB</p>
                  <p class="text-caption font-weight-bold mb-n1"><span  style="margin-left:19%;color:#383879">18GB</span>
                  <span  style="margin-left:2%;color:#BABED0">2GB</span><span  style="margin-left:5%;color:#6C85E6">84GB</span></p>
                  <div style="height:10vh;position:absolute:top:0;bottom:0" >
                      <div style="height:10vh;border-radius:15px;background-color:#DBE0EE" class="">
                          <div style="height:10vh;border-radius:15px;background-color:#383879;margin-left:20%">
                              <div style="height:10vh;border-radius:15px;background-color:#BABED0;margin-left:10%">
                                  <div style="height:10vh;border-radius:15px;background-color:#6C85E6;margin-left:5%">

                          </div>
                          </div>

                          </div>
                      </div>
                  </div>
                
                  <v-row style="position:absolute;bottom:0" no-gutters>
                    <p style="font-size:10px" class="mt-2"><v-icon size="12" color="#DBE0EE">mdi-square</v-icon>Free Space</p>
                    <v-spacer></v-spacer>
                    <p style="font-size:10px" class="mt-2"><v-icon size="12" color="#383879">mdi-square</v-icon>Swap File</p>
                    <v-spacer></v-spacer>
                    <p style="font-size:10px" class="mt-2"><v-icon size="12" color="#BABED0">mdi-square</v-icon>Cache</p>
                    <v-spacer></v-spacer>
                    <p style="font-size:10px" class="mt-2"><v-icon size="12" color="#6C85E6">mdi-square</v-icon>App Files</p>
                  </v-row>
              </v-card>
            </v-col>
            
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="12" xl="5" lg="5" class="">
        <v-card  class="ma-2">
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
