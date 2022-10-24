<template>
  <v-app dark>
    <v-app-bar fixed app>
      <v-btn icon @click.stop="">
        <v-icon>mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
      <v-spacer />
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script lang='ts'>
import Vue from 'vue';
export default Vue.extend({
  name: 'DefaultLayout',
  data () {
    return {
      title: 'Version Information',
    }
  },

})
</script>
