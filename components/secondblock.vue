<template>
  <v-container grid-list-xl style="padding: 0; padding-top: 12px;">
    <v-layout row wrap>
      <v-flex xs-col-md-6 style="padding: 0; max-width:50vw;">
          <img width="100%" src="../static/left.png">
      </v-flex>
      <v-flex xs-col-md-6 style="padding: 0; max-width:50vw;">
          <img width="100%" src="../static/right.png">
      </v-flex>
    </v-layout>
  </v-container>
</template>

<style scoped>

.layout {
  max-width:100vw;
  margin: 0px;
}

.container.grid-list-xl .layout:only-child {
    margin-top: -12px;
}

.container {
  padding: 0px;
  padding-top: 12px;
  margin-right: -12px;
  max-width: 100%;
}
</style>
