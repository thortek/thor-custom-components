<template>
<v-flex xs6>
<v-card>
<v-list>
          <v-list-tile
            v-for="(item, i) in items"
            :key="i"
            @click="showDetails"
          >
            <v-list-tile-action>
              <v-icon v-html="item.icon" color="blue">computer</v-icon>
            </v-list-tile-action>

            <v-list-tile-content>
              <v-list-tile-title v-text="item.title"></v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
        </v-list>

</v-card>
</v-flex>
</template>

<script>
export default {
    name: 'Servers',
data () {
    return {
        items: [{
            icon: 'computer',
            title: 'Server #1'
        },
        {
            icon: 'computer',
            title: 'Server #2'
        },
        {
            icon: 'computer',
            title: 'Server #3'
        }
        ,{
            icon: 'computer',
            title: 'Server #4'
        },
        {
            icon: 'computer',
            title: 'Server #5'
        }]
    }
},
methods: {
    showDetails(e) {
        console.log(e.target)
    }
}
}
</script>

<style>

</style>