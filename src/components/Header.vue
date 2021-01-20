<template>  
    <v-app-bar
      app
      color="red"
      flat
    >
      <v-tabs
        centered
        class="ml-n9"
        color="white"
      >
        <v-tab
          v-for="link in links"
          :key="link"
          class="tab"
        >
          {{ link }}
        </v-tab>
      </v-tabs>

      
    </v-app-bar>
</template>

<script>
export default {
    
    data: () => ({
      links: [
        'HOME',
        'CHI SONO',
        'SERVIZI',
        'PORTFOLIO',
        'CONTATTI',
      ],      
    }),
}
</script>

<style scoped>
  .tab {
    font-family:'Courier New', Courier, monospace;
    font-weight:900;
    font-size: 16px;
  }
  .tab:hover {
    border-bottom: 2px white solid;
  }

</style>