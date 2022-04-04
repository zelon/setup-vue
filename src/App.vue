<template>
  <v-app>
    <v-btn v-for="item in zelons" :key="item">{{ item }}</v-btn>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',

  data () {
    return {
      zelons: ['a', 'b', 'c']
    }
  },
})
</script>
