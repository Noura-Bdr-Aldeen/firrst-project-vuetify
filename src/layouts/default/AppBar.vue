<template>
  <v-app-bar>
    <v-btn>
      <v-img width="50" src=" ../../furniture/icon.jpg"></v-img>
    </v-btn>
          <v-app-bar-title>
      FURNITURE <STRONG>CALLERY</STRONG>
    </v-app-bar-title>

    <v-btn prepend-icon="mdi-heart" stacked="">
      <RouterLink to="/">Home</RouterLink>
    </v-btn>
    <v-btn prepend-icon="mdi-magnify" stacked="">
      <router-link to="/About">product</router-link>
    </v-btn>
  </v-app-bar>
</template>

<script setup>
//
</script>
