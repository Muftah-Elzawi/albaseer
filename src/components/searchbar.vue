<template>
    <nav>
        <v-toolbar app color="#007F9C"  style="padding:50px;">
            <v-spacer></v-spacer>
                <div class="Search-Div"> 
                    <v-autocomplete 
                    v-model="select"
                    :loading="loading"
                    :items="items"
                    :search-input.sync="search"
                    cache-items
                    class="mx-4 white--text"
                    append-icon="mdi-magnify"
                    flat
                    hide-no-data
                    hide-details
                    label="بحث"
                    solo-inverted
                    width="200">
                    </v-autocomplete>
                </div>
            <v-spacer></v-spacer>
        </v-toolbar>
    </nav>
</template>

<script>
export default {
    name:"Searchbar"
}
</script>

<style scoped>
.Search-Div{
padding-bottom: 50px;
}
.mx-4{
border-radius: 20px;
width: 500px;
}
/* border radius:50px; */
</style>