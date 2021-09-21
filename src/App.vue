<template>

  <v-app>

    

    <v-app-bar

      app

      color="primary"

      dark

    >

      <div color="primary" class="d-flex align-center">

                <v-img

          alt="Vuetify Name"

          class="shrink mt-1 hidden-sm-and-down"

          contain

          min-width="100"

          src="./assets/logo-vitens.png"

          width="100"

        />
 

        <v-container class="py-0 fill-height">

                        <v-tabs

        centered

        color="white"

        class = "primary"

      >

              <v-tab class = "primary">    

            <router-link  to="/" tag="button"> Home </router-link>

             </v-tab>

<v-tab class = "primary">  

           <router-link  to="/Modules" tag="button">Modules</router-link>

  </v-tab>

  <v-tab class = "primary">  

            <router-link  to="/Contact" tag="button"> Contact </router-link>

      </v-tab>

                        </v-tabs>

                        

        </v-container>

 



        





      </div>



      <v-spacer></v-spacer>



      <v-btn

        href="https://github.com/martidinho8/dashboard_2.git"

        target="_blank"

        text

      >

        <span class="mr-2">Latest Release</span>

        <v-icon>mdi-open-in-new</v-icon>

      </v-btn>

    </v-app-bar>



    <v-content>

      <router-view></router-view>

    </v-content>

  </v-app>

</template>



<script>



export default {

    data: () => ({

      links: [

        'Dashboard',

        'Messages',

        'Profile',

        'Updates',

      ],

    }),

  }

</script>

