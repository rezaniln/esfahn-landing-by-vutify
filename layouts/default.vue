<template>
  <v-app class="pa-0">
    
      <v-container fluid class="pa-0">
        <Nuxt />
        <Body />
         <Footer />
      </v-container>
   
    <v-footer></v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>
<style lang="scss">
:root {
  direction: rtl;
}
</style>
