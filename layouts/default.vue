<template>
  <v-app light>
   
    
    <firstblock/>

    <secondblock id="element"/>
    
    <v-footer :fixed="fixed" app>
      <span >&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<script>

import secondblock from '~/components/secondblock.vue'
import firstblock from '~/components/firstblock.vue'

  export default {
  components: {
    firstblock,
    secondblock
  },

    data() {
      
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>
