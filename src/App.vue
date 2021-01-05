<template>
  <v-app>
    <v-navigation-drawer app clipped permanent>
      <!-- -->
      <Nav />
    </v-navigation-drawer>

    <v-app-bar app color="primary" dark clipped-left>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <!-- <v-container fluid>
        <v-row>
        <v-col cols="3">
        <v-navigation-drawer>
        
        <Nav/>
       
       
        </v-navigation-drawer>
       </v-col>
       <v-col cols="9">
        <router-view></router-view>
        </v-col>
        <HelloWorld/>
        </v-row>
      </v-container> -->

      <v-container fluid>
        <router-view></router-view>
        <!-- <HelloWorld/> -->
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import Nav from "./components/Nav";

export default {
  name: "App",

  components: {
    // HelloWorld,
    Nav,
  },

  data: () => ({
    //
  }),
};
</script>
