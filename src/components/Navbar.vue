<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list dense>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-contact-mail</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>About</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

          <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-contact-mail</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Resturants</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

          <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-contact-mail</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Resturants</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

          <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-contact-mail</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      color="indigo"
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>Grub Scout</v-toolbar-title>
    </v-app-bar>

    <v-content>
      <v-container>
      <div class= "google-map-contiainer fill height">

        <v-row align="left" justify="center">

        </v-row>
      </div>
        

      </v-container>
    </v-content>

    
    <v-footer
      color="indigo"
      app
    >
      <span class="white--text">&copy; 2020 Grub Scout & Concrete Fox Design</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    name: "Navbar",
    props: {
      source: String,
    },
    data: () => ({
      drawer: null,
    }),
  }
</script>