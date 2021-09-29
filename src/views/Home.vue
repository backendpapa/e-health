<template>
  <div class="mt-4">
    <p class="text-h5 font-weight-bold">Dev Enviroment Services</p>
    <p class="text-caption mt-n3 grey--text">Your current development enviroment on internal network</p>

    <v-row class="" align="center"   justify="center" no-gutters>
      <v-col cols="12" xl="7" lg="7" class="" >
        <v-card elevation="1" class="pa-4 ma-2">
          <p class="text-h5 font-weight-bold" style=" color:#484C87;">Server Status</p>
          <v-row class="mb-n2" no-gutters>
         <v-col cols="5">
            <p class="text-caption mt-n2" style=" color:#484C87;"><v-icon style=" color:#484C87;" size="15">mdi-server</v-icon> Server-BRAVO-192.167</p>
            
         </v-col>
         <v-col cols="1" />
         <v-col cols="6" >
            <p style=" color:#484C87;" class="text-caption mt-n2 d-none d-sm-flex"><v-icon size="15" style=" color:#484C87;">mdi-database-settings-outline</v-icon> Server Account Quote</p>
         </v-col>
            </v-row>
          <v-row style="color:#484C87" no-gutters >
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
              
              <p style=" color:#484C87;" class="text-caption d-flex d-sm-none mt-3"><v-icon style=" color:#484C87;" size="15">mdi-database-settings-outline</v-icon> Server Account Quote</p>
              <v-card class="pa-2" flat style="height:30vh;background-color:#F3F5FD;border-radius:15px">
                  <p class="text-caption font-weight-bold" style=" color:#484C87;">Available 32.03GB from 120GB</p>
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
                    <p style="font-size:10px;color:#484C87;" class="mt-2"><v-icon size="12" color="#DBE0EE">mdi-square</v-icon> Free Space</p>
                    <v-spacer></v-spacer>
                    <p style="font-size:10px;color:#484C87;" class="mt-2"><v-icon size="12" color="#383879">mdi-square</v-icon> Swap File</p>
                    <v-spacer></v-spacer>
                    <p style="font-size:10px;color:#484C87;" class="mt-2"><v-icon size="12" color="#BABED0">mdi-square</v-icon> Cache</p>
                    <v-spacer></v-spacer>
                    <p  style="font-size:10px;color:#484C87;" class="mt-2"><v-icon size="12" color="#6C85E6">mdi-square</v-icon> App Files</p>
                  </v-row>
              </v-card>
            </v-col>
            
          </v-row>
        </v-card>
      </v-col>
      <v-col style="height:100%" cols="12" xl="5" lg="5" class="">
        <v-card style="height:50%"  class="ma-2 pa-4">
          <v-row no-gutters>
            <v-col cols="7">
              <p class="font-weight-bold" style=" color:#484C87;">Logged Commits</p>
              <p class="text-caption mt-n2" style=" color:#484C87;"><v-icon style=" color:#484C87;" size="12">mdi-github</v-icon> Github</p>
              <p style="font-size:10px; color:#484C87;"  class="mt-n2"><v-icon  size="12" color="#BDC1D2">mdi-circle</v-icon> Waiting for Review</p>
               <p style="font-size:10px;color:#484C87;" class="mt-n3"><v-icon size="12" color="#6C85E6">mdi-circle</v-icon> Accepted</p>
            </v-col>
            <v-col cols="5">
                <div class="">
                    <vc-donut
    background="white" foreground="#F3F5FD"
    :size="100" unit="px" :thickness="25"
 
    :sections="sections" :total="100"
    :start-angle="0" :auto-adjust-text-size="true"
    @section-click="handleSectionClick">
    <h1 class="text-h5 font-weight-bold" style="color:#484C87;">16</h1>
    <p style="font-size:8px;color:#484C87;" class="">Storage server</p>
  </vc-donut>
                </div>
            </v-col>
          </v-row>
        </v-card>
        <v-card style="height:50%"  class="ma-2 pa-4">
          <v-row no-gutters>
            <v-col cols="7">
              <p class="font-weight-bold mb-n1" style="color:#484C87;">Requesting New Services</p>
              <p class="text-caption mb-n1 " style="color:#484C87;">Are you looking for a new tool for your project?</p>
           
                <a href="" style="font-size:10px">Services list</a>
              
            </v-col>
            <v-col cols="5">
                <div class="">
                   
                      <v-img width=120 src="../assets/server.png"></v-img>
                  
                </div>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
    <v-row no-gutters align="center" justify="center">
        <v-col cols="12" class="" xl="2" lg="3" >
          <v-card  class=" ma-2" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px">
          <div class="pa-3">
            <p class="text-caption grey--text font-weight-bold" ><v-icon style="color:#484C87;" size="30">mdi-gitlab</v-icon> Gitlab</p>
          <p class="font-weight-bold" style="color:#484C87;">Gitlab</p>
          <p class="grey--text text-caption mb-n2 mt-n4">Version 1.2.4</p>
          </div>
          <v-btn color="#EBEEF7" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px;text-transform:none" block>
            <v-row no-gutters align="center" justify="center">
              <v-icon color="#ADE648" size="10">mdi-circle</v-icon>
              <p class="text-caption mt-4 ml-2" style="color:#484C87;">Running</p>
              <v-spacer></v-spacer>
              <v-icon size="10" style="color:#484C87;">mdi-information-outline</v-icon>
            </v-row>
          </v-btn>
        </v-card>
        </v-col>

        <v-col cols="12" class="" xl="2" lg="3" >
          <v-card  class=" ma-2" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px">
          <div class="pa-3">
            <p class="text-caption grey--text font-weight-bold"><v-icon style="color:#484C87;" size="30">mdi-oci</v-icon> Oci</p>
          <p class="font-weight-bold" style="color:#484C87;">Oracle Cloud </p>
          <p class="grey--text text-caption mb-n2 mt-n4">Version 1.1.4</p>
          </div>
          <v-btn color="#EBEEF7" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px;text-transform:none" block>
            <v-row no-gutters align="center" justify="center">
              <v-icon color="#ADE648" size="10">mdi-circle</v-icon>
              <p class="text-caption mt-4 ml-2" style="color:#484C87;">Running</p>
              <v-spacer></v-spacer>
              <v-icon size="10" style="color:#484C87;">mdi-information-outline</v-icon>
            </v-row>
          </v-btn>
        </v-card>
        </v-col>

         <v-col cols="12" class="" xl="2" lg="3" >
          <v-card   class=" ma-2" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px">
          <div class="pa-3">
            <p class="text-caption grey--text font-weight-bold"><v-icon color="red" size="30">mdi-kubernetes</v-icon> Kubernetes</p>
          <p class="font-weight-bold red--text"  >Kubernetes </p>
          <p class="grey--text text-caption mb-n2 mt-n4">Version 1.1.4</p>
          </div>
          <v-btn color="#FBC0C3" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px;text-transform:none" block>
            <v-row no-gutters align="center" justify="center">
              <v-icon color="red" size="10">mdi-circle</v-icon>
              <p class="text-caption mt-4 ml-2 red--text">Crashed</p>
              <v-spacer></v-spacer>
              <v-icon size="10" >mdi-information-outline</v-icon>
            </v-row>
          </v-btn>
        </v-card>
        </v-col>


        <v-col cols="12" class="" xl="2" lg="3" >
          <v-card  class=" ma-2" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px">
          <div class="pa-3">
            <p class="text-caption grey--text font-weight-bold"><v-icon style="color:#484C87;" size="30">mdi-apache-kafka</v-icon> Apache-kafka</p>
          <p class="font-weight-bold" style="color:#484C87;">Apache-Kafka </p>
          <p class="grey--text text-caption mb-n2 mt-n4">Version 2.1.3</p>
          </div>
          <v-btn color="#EBEEF7" style="border-bottom-right-radius:15px;border-bottom-left-radius:15px;text-transform:none" block>
            <v-row no-gutters align="center" justify="center">
              <v-icon color="#ADE648" size="10">mdi-circle</v-icon>
              <p class="text-caption mt-4 ml-2" style="color:#484C87;">Running</p>
              <v-spacer></v-spacer>
              <v-icon style="color:#484C87;" size="10">mdi-information-outline</v-icon>
            </v-row>
          </v-btn>
        </v-card>
        </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name:'Home',
  data(){
    return {
      sections: [
          
          { label: 'Green section', value: 50, color: '#6C85E6' },
          { label: 'Blue section', value: 10, color: '#CCCFDC' }
        ]
    }
  }
}
</script>
