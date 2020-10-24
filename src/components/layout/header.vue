<template>
    <nav>
    <v-app-bar
      app
      color="#007F9C"
      dark
      flat
      style="padding-bottom: 100px;"
    >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        <v-spacer></v-spacer>
      <div class="d-flex align-center">
        
        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="200"
          src="../../../public/1.png"
          width="200"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="http://localhost:8080/SignIn"
        target="_blank"
        text
      >
      <router-link></router-link>
        <!-- <v-icon>mdi-account-circle</v-icon> -->
        <v-img alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="28"
          src="../../../public/3.png"
          width="28"/>
      </v-btn>

    </v-app-bar>
      <v-navigation-drawer v-model="drawer" absolute bottom temporary>
          <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>
                <router-link to="/">الرئيسيه
                </router-link>
            </v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>
                <router-link to="/about">نبذه عن البصير
                </router-link>
            </v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
      </v-navigation-drawer>

    </nav>
</template>


<script>
export default {
    name: "Header",
    data: () => ({
      drawer: false,
      group: null,
    }),
}
</script>
<style scoped>

</style>