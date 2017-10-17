<template>
    <v-container grid-list-md text-xs-center>
        <v-layout row wrap>
            <v-flex xs12>
                <v-card color="grey lighten-4" flat>
                    <v-card-text>
                        <v-container fluid>
                            <v-layout row>
                                <v-text-field name="hotel_search" label="호텔검색" id="hotel_search"></v-text-field>
                            </v-layout>
                            <v-layout row>
                                <v-text-field name="hotel_search" label="호텔검색" id="hotel_search"></v-text-field>
                            </v-layout>
                        </v-container>
                    </v-card-text>                    
                </v-card>
            </v-flex>
        </v-layout>
        <v-layout row wrap>
            
        </v-layout>
    </v-container>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {}
  }
}
</script>