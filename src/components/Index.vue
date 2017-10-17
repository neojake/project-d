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
                        </v-container>
                    </v-card-text>
                </v-card>
            </v-flex>
        </v-layout>
        <v-layout>
            <v-data-table v-bind:headers="headers" :items="items" hide-actions class="elevation-1">
                <template slot="items" scope="props">
                    <td>{{ props.item.name }}</td>
                    <td class="text-xs-right">{{ props.item.calories }}</td>
                    <td class="text-xs-right">{{ props.item.fat }}</td>
                    <td class="text-xs-right">{{ props.item.carbs }}</td>
                    <td class="text-xs-right">{{ props.item.protein }}</td>
                    <td class="text-xs-right">{{ props.item.sodium }}</td>
                    <td class="text-xs-right">{{ props.item.calcium }}</td>
                    <td class="text-xs-right">{{ props.item.iron }}</td>
                </template>
            </v-data-table>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'app',
    data() {
        return {
            headers: [
                {
                    text: 'Dessert (100g serving)',
                    align: 'left',
                    sortable: false,
                    value: 'name'
                },
                { text: 'Calories', value: 'calories' },
                { text: 'Fat (g)', value: 'fat' },
                { text: 'Carbs (g)', value: 'carbs' },
                { text: 'Protein (g)', value: 'protein' },
                { text: 'Sodium (mg)', value: 'sodium' },
                { text: 'Calcium (%)', value: 'calcium' },
                { text: 'Iron (%)', value: 'iron' }
            ]
        }
    }
}
</script>