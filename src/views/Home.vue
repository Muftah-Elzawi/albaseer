<template>
  <div class="home">
    <v-container>
      <SlidShow/>
    </v-container>
   
  </div>
</template>

<script>
// @ is an alias to /src
import SlidShow from "../components/slidshow"

export default {
  name: 'Home',
  components: {
   SlidShow,
  },
  
}
</script>
