<template>
  <v-app>
    <Header/>
    <v-main>
      <Searchbar/>
     <router-view></router-view>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script>
import Header from './components/layout/header'
import Searchbar from './components/searchbar'
import Footer from './components/layout/footer'

export default {
  name: 'App',

  components: {
   Header,
   Searchbar,
   Footer,
  },

  data: () => ({
    //
  }),
};
</script>
