<template>
  <v-app>
    <div >
    <v-navigation-drawer
        permanent
        color="white"
        class="d-none d-sm-flex a "
        absolute
        style="color:#3E3C7D !important"
  
      >
        
         <p class="text-h6 font-weight-bold pa-3 mt-3">Dev/Env</p>

        <v-list
          nav
          dense  
rounded
        >
          <v-list-item  to="/" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/'?'#3E3C7D':'#bec4d6'">mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/'?'color:#3E3C7D':'color:#bec4d6'" class="font-weight-bold text-caption">Dashboard</v-list-item-title>
          </v-list-item>
          <v-list-item to="" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/t'?'#3E3C7D':'#bec4d6'">mdi-toolbox-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title class="font-weight-bold text-caption" :style="$route.path=='/t'?'color:#3E3C7D':'color:#bec4d6'">Services</v-list-item-title>
          </v-list-item>
          
          <v-list-item style="margin-top:5%" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/t'?'#3E3C7D':'#bec4d6'">mdi-cog-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/t'?'color:#3E3C7D':'color:#bec4d6'" class="font-weight-bold text-caption">Manage</v-list-item-title>
          </v-list-item>
        </v-list>

         <v-list
          nav
          dense  
          style="margin-top:15%"
rounded
        >
         <v-list-item  to="" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/t'?'#3E3C7D':'#bec4d6'">mdi-zip-disk</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/t'?'color:#3E3C7D':'color:#bec4d6'" class="font-weight-bold text-caption">Inser-Raise a ticket</v-list-item-title>
          </v-list-item>
          <v-list-item to="" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/t'?'#3E3C7D':'#bec4d6'">mdi-file-document</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/t'?'color:#3E3C7D':'color:#bec4d6'"  class="font-weight-bold text-caption">Documentation</v-list-item-title>
          </v-list-item>
         
         
        </v-list>
        <div>
          <p class="text-center"><v-avatar size="150">
            <v-img src="./assets/agent.png"></v-img>
          </v-avatar></p>
          <p class="text-center font-weight-bold text-caption mt-n7">Looking for an Answer?</p>
          <p style="font-size:10px;color:#3E3C7D;text-decoration:none" class="text-center mt-n5">Check on our <a href="" style="color:#3E3C7D;"> devlab</a></p>

          
        </div>
        <v-list dense rounded>
           <v-list-item to="" link>
            <v-list-item-icon>
              <v-icon :color="$route.path=='/t'?'#3E3C7D':'#bec4d6'">mdi-help-circle-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/t'?'color:#3E3C7D':'color:#bec4d6'"  class="font-weight-bold text-caption">Help Center</v-list-item-title>
          </v-list-item>
        </v-list>

      </v-navigation-drawer>
    </div>
    <v-main >
   <v-card  flat class="pa-4" color="#F7F7FB" style="height:100vh;">
    
      <!-- <div class=""> -->
      <!-- mobile -->
         <div class="d-flex d-sm-none" style="width:100%" >
           <div style="width:100%">
           <v-row  no-gutters class="ma-2 animate__animated animate__fadeIn " style="height:30px;width:100%" align="center" justify="center">
           <v-btn text plain icon small class="mt-n3 animate__animated animate__rubberBand"><v-icon size="20">mdi-bell-outline</v-icon></v-btn>
            <v-spacer></v-spacer>

           <div style="display:flex">
              
               <p class="text-caption font-weight-bold mt-1">Hi, Alex
                  
                  <v-menu
     
      rounded
      offset-y
      class="mr-4 white"
       :close-on-content-click="close"
       :close-on-click="close"
    >
      <template v-slot:activator="{ attrs, on }">
        <v-btn
          text
          class="ml-n2"
          icon
          v-bind="attrs"
          v-on="on"
        >
          <v-icon size="25">mdi-chevron-down</v-icon>
        </v-btn>
      </template>

      <v-list  rounded dense class="">
         <v-list-item @click="close=true" v-for="item in items" :key="item"  to="/t" link>
            <v-list-item-icon>
              <v-icon size="20" :color="$route.path=='/'?'#3E3C7D':'#bec4d6'">{{item.icon}}</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/'?'color:#3E3C7D':'color:#bec4d6'" class="font-weight-bold text-caption">{{item.title}}</v-list-item-title>
          </v-list-item>
      </v-list>
     
      <v-expansion-panels >
        <v-expansion-panel @click="close=false">
        <v-expansion-panel-header class="text-caption">More</v-expansion-panel-header>
        <v-expansion-panel-content class="animate__animated animate__fadeIn animate__slow ">
          <v-list   rounded dense class="ml-n6 mr-n4" flat>
         <v-list-item @click="close=true" v-for="item in items2" :key="item"  to="/t" link>
            <v-list-item-icon>
              <v-icon size="20" :color="$route.path=='/'?'#3E3C7D':'#bec4d6'">{{item.icon}}</v-icon>
            </v-list-item-icon>
            <v-list-item-title :style="$route.path=='/'?'color:#3E3C7D':'color:#bec4d6'" class="font-weight-bold text-caption">{{item.title}}</v-list-item-title>
          </v-list-item>
      </v-list>
        </v-expansion-panel-content>
      </v-expansion-panel>
      </v-expansion-panels>
    </v-menu> </p>
                <v-avatar class="mt-1"  rounded="true" size="30">
                    <v-img src="./assets/me.jpg"></v-img>
                </v-avatar>
             
           </div>
         </v-row>
         <v-text-field rounded  solo dense flat placeholder="Search" class="font-weight-bold text-caption mt-3 animate__animated animate__fadeIn animate__slow" append-icon="mdi-magnify" @click:append="hey" ></v-text-field>
           </div>
         </div>
         <!-- web menu2 -->
        <div class="d-none d-sm-flex animate__animated animate__fadeIn animate__slow" style="margin-left:18%">
           <v-row  no-gutters class="ma-2 " style="height:30px" align="center" justify="center">
              <v-text-field rounded   solo dense flat placeholder="Search" class="font-weight-bold " append-icon="mdi-magnify" @click:append="hey" ></v-text-field>
           <v-spacer></v-spacer>
            <v-spacer></v-spacer>

            <v-btn text plain icon small class="mt-n3 mr-3 text-caption animate__animated animate__rubberBand  "><v-icon class="" size="20">mdi-inbox-arrow-down</v-icon></v-btn>
             <v-btn text plain icon small class="mt-n3 mr-3 animate__animated animate__rubberBand "><v-icon class="" size="20">mdi-bell-outline</v-icon></v-btn>
             <v-btn text plain icon small class="mt-n3 mr-3 animate__animated animate__rubberBand "><v-icon class="" size="20">mdi-cog-outline</v-icon></v-btn>
              
                <p class="text-caption font-weight-bold mt-1">Hi, Alex
                  
                  <v-menu
     
      rounded="true"
      offset-y
    >
      <template v-slot:activator="{ attrs, on }">
        <v-btn
          text
          class="ml-n2"
          icon
          v-bind="attrs"
          v-on="on"
        >
          <v-icon size="25">mdi-chevron-down</v-icon>
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="item in items"
          :key="item"
          link
        >
          <v-list-item-title v-text="item"></v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu> </p>
                <v-avatar class="mt-n3"  rounded="true" size="30">
                    <v-img src="./assets/me.jpg"></v-img>
                </v-avatar>
            
           <!-- </div> -->
         </v-row>
        </div>
       <!-- </div> -->
      
      
     
        <router-view class="d-flex d-sm-none animate__animated animate__fadeIn animate__slower" style="overflow-y:scroll;height:80vh"/>
        <router-view class="d-none d-sm-flex mt-2 animate__animated animate__fadeIn animate__slower" style="overflow-y:scroll;height:80vh;margin-left:18.5%;"/>
     
    
   </v-card>
   </v-main>
  </v-app>
</template>

<script>
import './App.css'
export default {
  name: 'App',

  data: () => ({
    items:[
      {title:'Dashboard',icon:'mdi-home'},
      {title:'Services',icon:'mdi-toolbox-outline'},
      {title:'Manage',icon:'mdi-cog-outline'},
    
    ],
    items2:[
      {title:'Ticket',icon:'mdi-zip-disk'},
      {title:'Documentation',icon:'mdi-file-document '},
      
      
    
    ],
    close:true
  }),
  methods:{
    hey(){
      // alert("hey")
    }
  }
};
</script>
<style >

.v-navigation-drawer__border {
  width: 0px!important;
  background-color: red!important;
}
::-webkit-scrollbar {
  display: none;
}
.sh{
  color: #bec4d6;
}
</style>