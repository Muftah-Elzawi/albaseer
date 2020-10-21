<template>
  <v-app>
    <Header/>
    <v-main>
      <Searchbar/>
     <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import Header from './components/layout/header'
import Searchbar from './components/searchbar'

export default {
  name: 'App',

  components: {
   Header,
   Searchbar,
  },

  data: () => ({
    //
  }),
};
</script>
