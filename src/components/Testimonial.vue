<script setup></script>
<template>
     <div class="text-h3 ma-8"> Testimonial</div>
    <v-divider class="border-opacity-75 mb-6" color="secondary"></v-divider>
   <v-container>
      <v-row class="row-testimonial">
    <v-col  
    v-for="(variant, i) in variants"
        :key="i" cols="auto">
      <v-card width="200" height="200" class="overflow-auto">
        <v-card-text>
          <h3 class="pa-3">Opinion</h3>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis
          facilis dicta esse molestias vero hic laudantium provident nisi eos
          quasi iusto alias sequi, aut aliquid voluptatibus commodi! Minima, eum
          voluptates?
        </v-card-text>
      </v-card>
    </v-col>
</v-row>
</v-container>


</template>
<script setup>
const variants = ['outlined', 'outlined', 'outlined', 'outlined']
</script>