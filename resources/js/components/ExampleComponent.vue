<template>
<v-layout>
    <v-flex xs12 sm6 d-flex>
        <v-select
          :items="items"
          label="Standard"
        ></v-select>
    </v-flex>
    <v-flex xs12 sm6 d-flex>
        <v-select
          :items="items"
          label="Solo field"
          solo
        ></v-select>
    </v-flex>
</v-layout>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        },
    data () {
        return {
          items: ['Foo', 'Bar', 'Fizz', 'Buzz']
        }
    }

    }
</script>
