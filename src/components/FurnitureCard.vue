<script >
export default {
  data: () => ({
    show: false,
  }),
}
</script>
<template>
                <v-card 
                  class="mx-auto"
                  max-width="344"
            
                >
                  <v-img
                    src="../../furniture/sofa.jpg"
                    height="200px"
                    cover
                  ></v-img>
                  <v-card-title>
                    <slot name="title"></slot>
                  </v-card-title>
                  <v-card-subtitle>
                    <slot name="subtitle"></slot>
                  </v-card-subtitle>
                  <v-card-actions>
                    <v-btn
                      color="orange-lighten-2"
                      variant="text"
                    >
                      Explore
                    </v-btn>
                    <v-spacer></v-spacer>
                    <v-btn
                      :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
                      @click="show = !show"
                    ></v-btn>
                  </v-card-actions>
                  <v-expand-transition>
                    <div v-show="show">
                      <v-divider></v-divider>
                      <v-card-text>
                        household equipment, usually made of wood, metal, plastics, marble, glass, fabrics, or related materials and having a variety of different purposes
                      </v-card-text>
                    </div>
                  </v-expand-transition>
                </v-card>
</template>